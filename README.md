# Marker

Marker is a Typora-style Markdown editor for the Mac. You write in a live preview, and the formatting appears as you type. Themes start with Plain (the default), Night, Newsprint, and Solarized Light, then Classic, Library, Midnight, Blueprint, Sunday, Neon, Field, Matrix, Sorbet, and Dune.

This repo hosts Marker's downloads and its update feed. The source code lives elsewhere.

## Download

**[Download Marker (latest)](https://github.com/storybymarshall/marker-releases/releases/latest/download/Marker.zip)**

Marker needs macOS 13 Ventura or later on an Apple silicon Mac.

1. Open the downloaded `Marker.zip`. Your Mac unzips it into `Marker.app`.
2. Drag `Marker.app` into your **Applications** folder.
3. Open it. The first launch needs one extra step, explained below.

Older versions are on the [Releases](https://github.com/storybymarshall/marker-releases/releases) page.

## First launch: "Apple could not verify Marker…"

Marker isn't signed with an Apple Developer ID yet, so macOS blocks it the first time you open it. You only need to allow it once. After that, it opens normally, and updates install without asking again.

Pick one:

- **System Settings (macOS 15 Sequoia and later):** Open Marker once and click **Done** on the warning. Then go to **System Settings › Privacy & Security**, scroll down to the message about Marker, click **Open Anyway**, and confirm with your password.
- **Right-click (macOS 13 Ventura and macOS 14 Sonoma):** In Applications, right-click (or Control-click) Marker, choose **Open**, then click **Open** in the dialog.
- **Terminal (any version):** Run this command, then open Marker as usual:

  ```bash
  xattr -dr com.apple.quarantine /Applications/Marker.app
  ```

## Updates

Marker checks for updates by itself and offers to install new versions. You can also choose **Marker › Check for Updates…** at any time.

Every update is signed, and Marker verifies that signature before it installs anything. The feed is at <https://storybymarshall.github.io/marker-releases/appcast.xml>.
