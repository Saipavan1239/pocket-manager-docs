# Pocket Manager — Policy Website (v1.0.0)

Static GitHub Pages files for Pocket Manager.

## Files

- `index.html`
- `whats-new.html`
- `privacy.html`
- `terms.html`
- `licenses.html`
- `delete-account.html`
- `styles.css`

## What was corrected

This revision is based on the supplied agent context plus the reviewed app code/context.

- Removed unsupported claims about expense splitting, encrypted Room storage, 100% on-device security, and biometrics.
- Corrected the privacy description so it does not say all financial/application information stays on-device.
- Disclosed Firebase account/cloud synchronization for supported profile, statistics, daily statistics, and session information.
- Disclosed that the OCR flow uses Google ML Kit and that the reviewed code contains local OCR diagnostic logging.
- Kept the deletion page usable as an external account/data-deletion request resource.
- Avoided asserting an unverified SDP/SSP license; audit the exact shipped dependency versions.

## Before publishing

1. Replace `[YOUR_SUPPORT_EMAIL]` on all pages with your real support address.
2. Make sure the app has the matching in-app deletion flow if users can create accounts. Google Play requires account-creation apps to provide an in-app account-deletion path as well as an external web resource.
3. Re-check the Privacy Policy against the exact release build, especially Firebase products, diagnostics/logging, permissions, analytics/ads, and any cloud sync that is enabled at release.
4. Audit the exact Gradle dependency tree and include all required third-party license notices.
5. Keep this website repository separate from the private Android source repository.

## GitHub Pages

Create a public repository such as `pocket-manager-docs`, upload these files to the `main` branch, and enable GitHub Pages from Settings → Pages → Deploy from a branch.

After publishing, use the resulting public URLs in the app and Play Console, for example:

- `https://YOUR_GITHUB_USERNAME.github.io/pocket-manager-docs/privacy.html`
- `https://YOUR_GITHUB_USERNAME.github.io/pocket-manager-docs/terms.html`
- `https://YOUR_GITHUB_USERNAME.github.io/pocket-manager-docs/whats-new.html`
- `https://YOUR_GITHUB_USERNAME.github.io/pocket-manager-docs/licenses.html`
- `https://YOUR_GITHUB_USERNAME.github.io/pocket-manager-docs/delete-account.html`
