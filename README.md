# Axiom for Android: downloads

**Download page: https://nahimjmu.github.io/axiom-android/**

This repository only publishes the Axiom Android app for teachers and parents (the
`downloads` branch, served by GitHub Pages). It holds no source code: releases are built,
tested and signed in the private Axiom repository, and pushed here automatically.

- `downloads` branch: the APK (`axiom.apk`), `latest.json` (the version the installed
  apps check for, plus the school server's address) and the download page. Replaced on
  every release.
- `.github/workflows/keep-awake.yml`: during school hours (06:30–19:30 IST, Mon–Sat) it
  pings the school site every 10 minutes, so the free host doesn't put it to sleep and
  the first teacher of the morning doesn't wait. Set the repository variable `SITE_URL`
  to the site's address.
