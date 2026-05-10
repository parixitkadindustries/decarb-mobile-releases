# decarb-mobile-releases

Public binary releases for the DeCarb Mobile (Flutter) operator app.

This repo holds **APKs only** — no source code. Source lives in the private
`DeCarbMobile_flutter` repo. The split exists so the in-app update banner
and the install landing page can fetch APKs over plain HTTPS without an
auth token.

Each release is a single AAB or APK named `app-release.apk`, tagged
`decarb-mobile-vX.Y.Z+B`. The Flutter app reads
`/app_settings/mobile_versions` from Firestore (project
`decarb-fleet-f3b9c`) to find the latest release URL.

See https://decarbonmachine.web.app/install for the customer-facing
download page.
