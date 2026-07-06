# Day 06 - Browser History and Download Forensics

## Introduction

Web browsers record a significant amount of user activity during
everyday use. Browser history, download records, bookmarks, and cached
data are frequently examined during digital forensic investigations
because they help investigators reconstruct browsing behavior and user
intent.

This investigation focused on Google Chrome running on Windows 11. The
objective was to examine browser history and download artifacts using
Chrome's built-in pages.

## Investigation Objectives

-   Examine browser history.
-   Review download history.
-   Identify browsing patterns.
-   Understand the forensic value of browser artifacts.

## Investigation Environment

  Component            Details
  -------------------- ---------------------------
  Operating System     Windows 11
  Browser              Google Chrome
  Investigation Type   Browser Artifact Analysis

## Browser History Investigation

The Chrome History page (`chrome://history`) was examined.

### Observations

Most recent website:

-   ChatGPT

Second website:

-   Google Narikootam YouTube Channel

History contained a very large number of entries, indicating long-term
browser usage.

### Forensic Importance

Browser history helps investigators determine:

-   Websites visited
-   Research activity
-   Browsing timelines
-   User interests

## Download History Investigation

The Chrome Downloads page (`chrome://downloads`) was examined.

### Observations

Most recent download:

-   Digital Forensics Markdown project files

Download date:

-   30 June 2026

A large number of downloads from different categories were present.

### Forensic Importance

Download history provides evidence of:

-   Files acquired from the internet
-   Project activity
-   Software downloads
-   User intent

## Evidence Summary

  Artifact          Observation
  ----------------- ----------------------------------
  Browser History   Large history database
  Recent Website    ChatGPT
  Second Website    Google Narikootam YouTube
  Downloads         Large number of records
  Latest Download   Digital Forensics Markdown files

## Key Findings

-   Active browser usage was identified.
-   Technical research and learning activity was observed.
-   Project-related downloads were present.
-   Browser artifacts supported previous Registry and Prefetch
    investigations.

## Lessons Learned

-   Browser history is valuable for reconstructing user activity.
-   Download records can reveal project work and file acquisition.
-   Browser artifacts should be correlated with Registry and Prefetch
    evidence.

## Conclusion

This investigation demonstrated that Google Chrome stores valuable
evidence regarding browsing history and downloads. These artifacts
provide investigators with useful information about browsing behavior
and can be correlated with other forensic evidence to reconstruct user
activity.

## Screenshot Placeholders

-   Chrome History
-   Chrome Downloads
-   Browser History Overview
