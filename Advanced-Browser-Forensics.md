# Day 07 - Advanced Browser Forensics

## Introduction

Modern web browsers retain several artifacts beyond browsing history.
Bookmarks and site data (cookies and stored website data) provide
valuable information about a user's browsing habits, frequently accessed
services, and long-term activity. During this investigation, Google
Chrome was examined to understand the forensic value of these artifacts.

## Investigation Objectives

-   Examine Chrome bookmarks.
-   Review stored website data.
-   Understand the forensic value of browser artifacts.
-   Correlate findings with previous investigations.

## Investigation Environment

  Component          Details
  ------------------ ---------------------------
  Operating System   Windows 11
  Browser            Google Chrome
  Investigation      Browser Artifact Analysis

## Bookmark Investigation

The Chrome bookmark manager (`chrome://bookmarks`) was examined.

### Observations

Approximate bookmarks:

-   20--25

Frequently bookmarked websites:

-   GitHub
-   Render
-   Vercel
-   YouTube

### Forensic Importance

Bookmarks often represent websites the user accesses repeatedly and may
reveal long-term interests, work platforms, and frequently used online
services.

------------------------------------------------------------------------

## Site Data / Cookies Investigation

The Chrome site data page (`chrome://settings/content/all`) was
examined.

### Observations

-   A large number of websites had stored site data.
-   Common services included:
    -   ChatGPT
    -   GitHub
    -   Google
    -   YouTube

### Forensic Importance

Cookies and stored site data may indicate repeated website usage,
authenticated sessions, and long-term browser activity.

------------------------------------------------------------------------

## Evidence Correlation

The browser findings support previous investigations:

  Previous Artifact   Supporting Observation
  ------------------- -----------------------------------
  RecentDocs          Development-related file types
  Prefetch            CODE.EXE and CHROME.EXE execution
  Browser Bookmarks   GitHub, Render, Vercel
  Site Data           Large number of active websites

Together, these artifacts indicate software development, technical
learning, and regular browser usage.

------------------------------------------------------------------------

## Key Findings

-   Approximately 20--25 bookmarks were present.
-   Development platforms such as GitHub, Render, and Vercel were
    bookmarked.
-   Numerous websites stored browser data.
-   Browser artifacts were consistent with previous Registry and
    Prefetch evidence.

------------------------------------------------------------------------

## Lessons Learned

-   Bookmarks reveal long-term browsing preferences.
-   Cookies and site data provide valuable supporting evidence.
-   Multiple browser artifacts should always be correlated with system
    artifacts during an investigation.

------------------------------------------------------------------------

## Conclusion

This investigation demonstrated that browser bookmarks and stored site
data are valuable forensic artifacts. Although they do not prove every
user action individually, they contribute significantly to
reconstructing browsing behavior when combined with Registry, Prefetch,
and browser history evidence.

## Screenshot Placeholders

-   Chrome Bookmarks
-   Chrome Site Data
-   Browser Settings Overview
