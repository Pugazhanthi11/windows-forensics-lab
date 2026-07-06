# Day 05 - Windows Prefetch Forensics

## Introduction

Windows Prefetch is a performance feature that stores information about
applications executed on the system. While its primary purpose is to
improve application startup time, Prefetch files are extremely valuable
during digital forensic investigations because they provide evidence
that a program has been executed.

This investigation was performed on a Windows 11 system using the
Prefetch folder to understand how application execution artifacts are
stored and interpreted.

## Investigation Objectives

-   Understand Windows Prefetch.
-   Identify executed applications.
-   Correlate Prefetch evidence with previous Registry findings.
-   Document forensic observations.

## Investigation Environment

  Component            Details
  -------------------- -------------------------------------
  Operating System     Windows 11
  Evidence Location    C:`\Windows`{=tex}`\Prefetch`{=tex}
  Investigation Type   Application Execution Analysis

## Prefetch Overview

Each Prefetch file ends with the `.pf` extension and is usually named
after the executable that generated it.

Examples observed:

-   CMD.EXE
-   CODE.EXE
-   CHROME.EXE

## Investigation Findings

### CMD.EXE

Observed Prefetch files:

-   CMD.EXE-0BD30981.pf
-   CMD.EXE-6D6290C5.pf

Latest observed modification:

**01-07-2026 09:07 PM**

**Finding:** Evidence confirms that Command Prompt was executed on the
system. This finding also supports the RunMRU artifact examined during
Day 04.

------------------------------------------------------------------------

### CODE.EXE

Observed:

-   7 CODE.EXE Prefetch files

Latest observed modification:

**30-06-2026 12:04 PM**

**Finding:** Multiple Prefetch entries indicate repeated use of Visual
Studio Code, which is consistent with software development activity.

------------------------------------------------------------------------

### CHROME.EXE

Observed:

-   12 CHROME.EXE Prefetch files

Latest observed modification:

**01-07-2026 09:09 PM**

**Finding:** Google Chrome was executed frequently, indicating regular
browser usage.

## Evidence Correlation

Evidence from previous investigations supports these observations:

  Artifact     Observation
  ------------ ------------------------------------------------------
  RunMRU       cmd executed
  RecentDocs   Source code and document files accessed
  Prefetch     CMD.EXE, CODE.EXE and CHROME.EXE execution confirmed

Using multiple independent artifacts increases confidence in forensic
conclusions.

## Key Findings

-   Command Prompt execution confirmed.
-   Visual Studio Code used repeatedly.
-   Google Chrome executed frequently.
-   Prefetch supports Registry-based evidence collected during Day 04.

## Lessons Learned

-   Prefetch provides reliable evidence of application execution.
-   Multiple forensic artifacts should be correlated instead of relying
    on a single source.
-   Prefetch is useful during malware investigations and incident
    response.

## Conclusion

This investigation demonstrated how Windows Prefetch files can be used
to identify executed applications and reconstruct user activity. By
correlating Prefetch data with Registry artifacts collected previously,
it was possible to build a stronger evidence-based understanding of
system usage.

## Screenshot Placeholders

-   Prefetch Folder
-   CMD.EXE Prefetch
-   CODE.EXE Prefetch
-   CHROME.EXE Prefetch
