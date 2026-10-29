# BearOS

BearOS is the admin interface for a BearMail server. It is a modified community build of [Stalwart WebUI](https://github.com/stalwartlabs/webui) 2.0.2.

The visible product name is BearOS. File copyright headers and the license texts are unchanged. This build chooses the AGPL-3.0-only side of the upstream dual license.

Copyright (C) 2024, Stalwart Labs LLC.

## License

This project is licensed under the **GNU Affero General Public License v3.0** (AGPL-3.0-only). The full text is in [LICENSES/AGPL-3.0-only.txt](./LICENSES/AGPL-3.0-only.txt).

Upstream also offers a proprietary Stalwart Enterprise License. This BearOS repository does not use that license. See [LICENSES/LicenseRef-SEL.txt](./LICENSES/LicenseRef-SEL.txt) only as the upstream text that remains in the tree.

## Build

Requires Node.js 22.

```sh
npm ci
npm run build
cd dist && zip -r ../webui.zip .
```

Stalwart fetches `webui.zip` from this repository's latest GitHub release and serves it at `/admin` and `/account`.
