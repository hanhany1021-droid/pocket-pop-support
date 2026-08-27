# Project Context

- Status: Active public support site for Pocket Pop 1.0
- Last reviewed: 2026-08-27

## Intent

Provide stable, public, authentication-free privacy and support URLs for Pocket Pop users and App Store review.

## Background

Pocket Pop turns an iPhone into a small tactile toy inspired by the familiar satisfaction of pressing transparent plastic bubble wrap. Its first release is a free, offline iPhone app centered on sound, visuals, and Core Haptics. Apple requires a public privacy-policy URL and a support URL for distribution, so these operational pages are kept separately from the private application source.

## Audience and job to be done

- Pocket Pop users need a concise explanation of privacy behavior and a route for reporting problems.
- App Review needs stable public pages that accurately match the submitted binary and App Privacy answers.
- Maintainers need an auditable place to update policy and support text before release behavior changes.

## Current factual scope

- A static English landing page, privacy policy, and support page.
- GitHub Issues is the public support intake mechanism.
- GitHub Pages is the hosting mechanism.
- Pocket Pop 1.0 is represented as offline and collecting no personal or usage data.

## Boundaries

- This repository does not contain the iOS source, signing material, reviewer contact details, user records, or private release artifacts.
- Do not publish screenshots, logs, issue attachments, or diagnostics containing personal or sensitive information.
- The privacy policy must never promise behavior that is not verified against the current app binary and third-party dependencies.
- If the app adds accounts, networking, analytics, advertising, tracking, third-party SDKs, or new device permissions, update the app implementation review, App Store privacy answers, and this site together before release.

## Acceptance baseline

- The home, privacy, and support pages load without authentication over HTTPS.
- Internal links resolve, and the support tracker is publicly reachable.
- Policy claims match the submitted Pocket Pop version.
- No credentials or private source are present in the repository.

## Success hypotheses

These are not measured results:

- A short policy makes Pocket Pop's offline privacy boundary understandable.
- A structured issue prompt improves the usefulness of support reports.
- Separating the public site from private source reduces accidental code disclosure.

## Risks and open questions

- GitHub availability is an external dependency for support and policy access.
- Public issues may attract spam or users may post sensitive information despite warnings.
- Future app features may make the current no-data statement stale.

## Update triggers

Review this document and the public pages whenever privacy behavior, permissions, support channels, hosting, App Store disclosures, or release scope changes.
