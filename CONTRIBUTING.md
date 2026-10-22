# Contributing to Bipe

Thank you for helping. This file applies to every repo in the bipe-chat organisation. A repo can add its own rules on top.

## Before you start

- For anything bigger than a small fix, open an issue first. Say what you want to change and why. Bipe keeps a small core on purpose, so some good ideas will wait.
- In the app forks (bipe-ios, bipe-android), Bipe code lives in its own module and Element's code gets small hooks only. A fix to Element's code belongs upstream at [element-hq](https://github.com/element-hq) first.
- Each repo has an `AGENTS.md` with its commands, rules and build gate. Read it before you open a pull request.

## Sign off your commits (DCO)

Bipe uses the [Developer Certificate of Origin](https://developercertificate.org/). Each commit must end with a sign-off line:

```
Signed-off-by: Your Name <you@example.com>
```

`git commit -s` adds it. The line says that you wrote the change, or have the right to submit it, under the repo's licence. There is no separate agreement to sign.

## Licence

- **Bipe code** (Bipe's own repos, BipeKit in bipe-ios, `libraries/bipe*` in bipe-android, and Bipe's own app clients): your contribution is licensed under AGPL-3.0-only with the [app store permission](APP-STORE-PERMISSION.md). The permission lets Bipe and anyone else ship the code through app stores such as the Apple App Store.
- **Element code** in bipe-ios and bipe-android: your contribution is licensed under that code's licence (AGPL-3.0). Better: send the change to [element-hq](https://github.com/element-hq) first.

The DCO sign-off confirms that you have the right to license your change on these terms.

## Security

Do not report security problems in public issues. See [SECURITY.md](SECURITY.md).

## Conduct

See [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).
