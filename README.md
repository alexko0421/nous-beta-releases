# Nous Beta releases

Update packages for the Nous Beta macOS app, served to [Sparkle](https://sparkle-project.org)
through the Nous managed API's appcast feed.

**This repository holds release binaries only. No source code lives here.**

- Each release tag is a build number (`b24`, `b25`, …) and carries one `.zip`.
- The zips are notarized and stapled, and signed with Sparkle's EdDSA key. The
  app has the matching public key compiled in, so a package that is not signed
  by that key is refused at install time — a public download URL is not a trust
  boundary here.
- The appcast (`/api/appcast`) is what decides which build is offered. Adding a
  release here does not publish it on its own.

Source lives in a private repository.
