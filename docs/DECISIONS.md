# Decisions

This log is append-only. If a decision changes, mark it superseded and add a new entry.

## D-001: Separate public support site from private app source

- Date: 2026-08-27
- Status: Accepted
- Context: App Store distribution needs public privacy and support URLs, while the Pocket Pop application source is private.
- Decision: Host only static support and policy material in this public repository.
- Reason: Public pages remain accessible without exposing implementation or release material.
- Consequences: App behavior and public policy must be reviewed together before each privacy-relevant release.

## D-002: Use GitHub Pages and Issues

- Date: 2026-08-27
- Status: Accepted
- Context: Pocket Pop 1.0 needs a low-maintenance public host and a support route.
- Decision: Publish static files from the default branch through GitHub Pages and use repository Issues for support.
- Reason: Both mechanisms are simple, public, and require no data-collection backend.
- Consequences: GitHub availability becomes an operational dependency, and maintainers must watch public issues for sensitive disclosures.

## D-003: Keep the site free of user data and credentials

- Date: 2026-08-27
- Status: Accepted
- Context: The public repository does not need customer data, App Store reviewer details, analytics, or secrets.
- Decision: Do not store such material here.
- Reason: This minimizes privacy and disclosure risk and stays consistent with Pocket Pop's offline product boundary.
- Consequences: Support diagnostics must be voluntarily provided through public issues with a warning not to include sensitive information.

## D-004: Explain Apple-managed material purchases before the 1.5 review

- Date: 2026-10-29
- Status: Accepted
- Context: Popwrap 1.5 adds optional non-consumable wood and metal materials. The former “completely offline” description no longer covers price loading, purchases or restores.
- Decision: Keep classic gameplay free and offline. Explain that Apple handles optional one-time purchases and restores, that the developer does not receive Apple Account credentials or card details, and that verified ownership is checked on the device. Document the free two-bubble trial, separate/bundle purchases, no top-up offer and public-support privacy boundary.
- Reason: Users and App Review need policy and support text that matches the submitted app without confusing Apple payment handling with developer data collection.
- Consequences: Pages explicitly mark these purchase features as prepared for version 1.5 until availability is verified. Publication of support text is not evidence that the app is uploaded, approved or released. No app source, credentials or private review data are published.
