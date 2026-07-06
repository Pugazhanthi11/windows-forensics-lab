# Day 09 - Windows Shortcut (LNK) File Forensics

## Introduction

Windows shortcut (.LNK) files are valuable forensic artifacts because
they can reveal evidence that a file, folder, or application was
accessed by a user. Even if the original file has been moved or deleted,
the shortcut may still contain useful metadata.

This investigation introduces the purpose of LNK files and demonstrates
how they can support timeline reconstruction during a digital forensic
investigation.

## Investigation Objectives

-   Understand the purpose of Windows shortcut files.
-   Learn where shortcut files are commonly stored.
-   Examine shortcut file properties.
-   Understand the forensic value of LNK artifacts.

## Investigation Environment

  Component            Details
  -------------------- -------------------------
  Operating System     Windows 11
  Artifact             Windows Shortcut (.LNK)
  Investigation Type   User Activity Analysis

------------------------------------------------------------------------

## What is a LNK File?

A shortcut (.lnk) file is created by Windows to provide quick access to
a file, folder, or application. Besides acting as a shortcut, it stores
metadata that may include:

-   Original target path
-   Target file name
-   Last accessed information
-   Creation and modification details
-   Volume information

These details make shortcut files valuable during forensic
investigations.

------------------------------------------------------------------------

## Common Locations

Investigators commonly examine shortcut files in locations such as:

-   Desktop
-   Start Menu
-   Recent Items
-   User profile folders

The **Recent Items** folder is especially useful because it may contain
shortcuts to recently opened files.

------------------------------------------------------------------------

## Practical Investigation

During this stage of the learning journey, the objective was to
understand where LNK files are located and why they are important.

The investigation focused on:

-   Identifying shortcut files created by Windows.
-   Understanding the metadata stored inside shortcuts.
-   Learning how shortcut artifacts support evidence correlation.

This serves as the foundation for more advanced shortcut analysis using
forensic tools later in the journey.

------------------------------------------------------------------------

## Forensic Importance

LNK files may help investigators answer questions such as:

-   Which files were opened?
-   Which applications were launched?
-   Was a removable USB device used?
-   What was the original location of a file?

Because of this, shortcut files are frequently examined in incident
response, malware analysis, and user activity investigations.

------------------------------------------------------------------------

## Key Findings

-   Windows automatically creates shortcut artifacts in many situations.
-   Shortcut files preserve useful metadata.
-   LNK artifacts can support timeline reconstruction.
-   LNK analysis should be correlated with Registry, Prefetch, Event
    Logs, and Browser artifacts.

------------------------------------------------------------------------

## Lessons Learned

-   Shortcut files are evidence, not just convenience features.
-   Metadata is often as valuable as the original file.
-   Multiple artifacts together provide stronger forensic conclusions.

------------------------------------------------------------------------

## Conclusion

This investigation introduced the role of Windows shortcut files in
digital forensics. Although this was a foundational exercise, it
established how LNK artifacts contribute to reconstructing user
activity. Future investigations will involve parsing shortcut metadata
using dedicated forensic tools and correlating it with other Windows
artifacts.

------------------------------------------------------------------------

## Screenshot Placeholders

-   Desktop Shortcut Example
-   Shortcut Properties
-   Recent Items Folder
