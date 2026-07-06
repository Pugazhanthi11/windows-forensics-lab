# Day 04 - Windows Registry Forensics

## Introduction

The Windows Registry is one of the most valuable sources of evidence in
a Windows operating system. It stores configuration data for the
operating system, installed software, hardware, and user activity.
During digital forensic investigations, Registry artifacts help
investigators reconstruct user actions and understand how a system has
been used.

This investigation was performed on a Windows 11 computer as part of my
Digital Forensics learning journey.

## Investigation Objectives

-   Understand the Windows Registry.
-   Examine RunMRU, RecentDocs, UserAssist, TypedPaths and
    WordWheelQuery.
-   Document observations and forensic significance.

## Investigation Environment

  Component          Details
  ------------------ ---------------------------
  Operating System   Windows 11
  Tool               Registry Editor (regedit)

## RunMRU

Location:
`HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\RunMRU`

Observed commands: - cmd - temp - %temp% - recent

MRUList: `dabc`

**Finding:** The Registry confirmed manual execution of Run dialog
commands.

## RecentDocs

Observed file types: - .txt - .pdf - .png - .py - .md - .cpp - .dart -
.docx

**Finding:** RecentDocs confirmed recent access to development files,
documents and images.

## UserAssist

UserAssist entries were present and encoded using ROT13.

**Finding:** Evidence of application execution was available.

## TypedPaths

No manually typed File Explorer paths were recorded.

## WordWheelQuery

The artifact was not present during the investigation.

## Evidence Summary

  Artifact         Result
  ---------------- -------------
  RunMRU           Present
  RecentDocs       Present
  UserAssist       Present
  TypedPaths       Empty
  WordWheelQuery   Not Present

## Key Findings

-   Run dialog history was recovered.
-   Recently opened file types were identified.
-   Application execution artifacts were present.
-   Empty and missing artifacts were documented.

## Conclusion

This investigation demonstrated how Registry artifacts preserve user
activity. Even a small number of Registry keys provided useful evidence
that could assist in reconstructing user actions during a forensic
investigation.

## Screenshot Placeholders

-   Registry Editor
-   RunMRU
-   RecentDocs
-   UserAssist
-   TypedPaths
