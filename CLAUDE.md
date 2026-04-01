# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is the **public release distribution repository** for OrbCapture — a macOS screen recording app. It contains no source code. The actual app source lives in a private repository; compiled `.zip` releases are published here.

## Release Workflow

To publish a new release:
1. Build and export `OrbCapture.app` from the private source repo
2. Zip it: `zip -r OrbCapture-vX.Y.Z.zip OrbCapture.app`
3. Add the zip to this repo and commit
4. Remove the previous version's zip if superseded (keep only the latest)
5. Update README.md if the version reference in the download example is stale

## App Details

- **Bundle ID:** `com.richard.orbcapture`
- **Min macOS:** 14.0 (Sonoma)
- **Permissions needed:** Screen Capture, Camera, Microphone
- **Required permissions** are declared in `Info.plist` inside the app bundle

## Remote

- GitHub: `https://github.com/lgh521/orbCapture-public`
