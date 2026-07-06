# Day 08 - Recycle Bin Forensics

## Introduction

Deleting a file in Windows does not immediately remove it from the
storage device. Instead, Windows moves the file to the Recycle Bin,
where it can often be recovered until the Recycle Bin is emptied. This
behavior makes the Recycle Bin an important source of digital evidence
during forensic investigations.

The purpose of this investigation was to understand how deleted files
are handled by Windows and what information can be recovered from the
Recycle Bin.

## Investigation Objectives

-   Understand the forensic importance of the Recycle Bin.
-   Create a controlled evidence file.
-   Delete the file and observe its behavior.
-   Document the available forensic artifacts.

## Investigation Environment

  Component            Details
  -------------------- ---------------------
  Operating System     Windows 11
  Investigation Area   Windows Recycle Bin
  Evidence File        forensics_day8.txt

------------------------------------------------------------------------

## Controlled Experiment

A text file named **forensics_day8.txt** was created on the Desktop for
this investigation.

The following text was added to the file:

> This file is created for Day 08 Recycle Bin Investigation.

After confirming that the file was saved successfully, it was deleted
using the standard Windows Delete option.

------------------------------------------------------------------------

## Evidence Collected

### File Name

forensics_day8.txt

### Original Location

C:`\Users`{=tex}`\pugaz`{=tex}`\OneDrive`{=tex}`\Desktop`{=tex}

### File Type

Text Document

### File Size

1 KB

### Date Deleted

02-07-2026 09:02 PM

### Observation

The deleted file appeared inside the Recycle Bin immediately after
deletion and was still available for restoration.

------------------------------------------------------------------------

## Forensic Analysis

This investigation demonstrated that deleting a file does not
immediately erase it from the system.

Instead, Windows preserved important information including:

-   Original file location
-   File name
-   File type
-   Deletion timestamp
-   Recovery option

These artifacts may help investigators reconstruct user actions during
an investigation.

------------------------------------------------------------------------

## Timeline Reconstruction

  Event                         Time
  ----------------------------- ----------------------------
  File Created                  02-07-2026
  File Saved                    02-07-2026
  File Deleted                  02-07-2026 09:02 PM
  File Present in Recycle Bin   Immediately after deletion

------------------------------------------------------------------------

## Key Findings

-   Deleted files remain in the Recycle Bin until permanently removed.
-   Original file information is preserved.
-   Deletion timestamps are valuable forensic evidence.
-   Controlled experiments help understand how Windows manages deleted
    files.

------------------------------------------------------------------------

## Lessons Learned

-   Deleting a file is not the same as permanently destroying it.
-   The Recycle Bin is an important forensic artifact.
-   Timeline reconstruction becomes easier when deletion timestamps are
    available.
-   Deleted file investigations should be correlated with other forensic
    artifacts.

------------------------------------------------------------------------

## Conclusion

The Recycle Bin provides investigators with valuable information about
deleted files and user actions. This practical investigation
demonstrated how Windows preserves deleted file metadata and how
investigators can use this information to reconstruct events during a
digital forensic examination.

------------------------------------------------------------------------

## Screenshot Placeholders

-   Recycle Bin Overview
-   forensics_day8.txt inside Recycle Bin
-   File Properties (Optional)
