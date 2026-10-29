# Project Context

- Status: Active public support site for Popwrap; updated for the version 1.5 App Review submission, not an announcement of availability
- Last reviewed: 2026-10-29

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
- Classic play is free and runs offline on iPhone and iPad; settings and gameplay statistics stay on the device.
- Version 1.5 adds optional one-time wood/metal purchases through Apple StoreKit, with two-bubble trials in all three modes. Prices, purchases and restores need internet access.
- The developer does not collect app activity or receive Apple Account credentials or card details. Apple processes purchases; verified transactions are checked on the device, not uploaded to a developer server.
- GitHub Issues is an external, potentially public service. Users must not include Apple IDs, receipts, payment details or other sensitive information.
- The three pages identify material purchases as being prepared for version 1.5. No app upload, review approval or release is claimed by this site update.

## Boundaries

- This repository does not contain the iOS source, signing material, reviewer contact details, user records, or private release artifacts.
- Do not publish screenshots, logs, issue attachments, or diagnostics containing personal or sensitive information.
- The privacy policy must never promise behavior that is not verified against the current app binary and third-party dependencies.
- Review new or changed accounts, networking, payments, analytics, advertising, tracking, third-party SDKs or device permissions against the app implementation and App Store privacy answers before release. Apple-managed payments do not imply a developer-operated account or payment backend.

## Acceptance baseline

- The home, privacy, and support pages load without authentication over HTTPS.
- Internal links resolve, and the support tracker is publicly reachable.
- Policy claims match the submitted Pocket Pop version.
- No credentials or private source are present in the repository.

## Success hypotheses

These are not measured results:

- A short policy makes the boundary between offline play and Apple-managed purchases understandable.
- A structured issue prompt improves the usefulness of support reports.
- Separating the public site from private source reduces accidental code disclosure.

## Risks and open questions

- GitHub availability is an external dependency for support and policy access.
- Public issues may attract spam or users may post sensitive information despite warnings.
- Future app features may make the current no-data statement stale.

## Update triggers

Review this document and the public pages whenever privacy behavior, permissions, support channels, hosting, App Store disclosures, or release scope changes.
