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


## GitHub Pages

Create a public repository such as `pocket-manager-docs`, upload these files to the `main` branch, and enable GitHub Pages from Settings → Pages → Deploy from a branch.

After publishing, use the resulting public URLs in the app and Play Console, for example:

- `https://YOUR_GITHUB_USERNAME.github.io/pocket-manager-docs/privacy.html`
- `https://YOUR_GITHUB_USERNAME.github.io/pocket-manager-docs/terms.html`
- `https://YOUR_GITHUB_USERNAME.github.io/pocket-manager-docs/whats-new.html`
- `https://YOUR_GITHUB_USERNAME.github.io/pocket-manager-docs/licenses.html`
- `https://YOUR_GITHUB_USERNAME.github.io/pocket-manager-docs/delete-account.html`
