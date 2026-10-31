# Contributing to Bipe

Thank you for helping. This file applies to every repo in the bipe-chat organisation. A repo can add its own rules on top.

Issues and discussion in Portuguese are welcome. Code, commit messages and code comments are in English.

## Where to start

| Repo | What it is | Stack |
|---|---|---|
| [bipe-app](https://github.com/bipe-chat/bipe-app) | The app for iPhone and Android | SwiftUI, Jetpack Compose, matrix-rust-sdk |
| [bipe-shared](https://github.com/bipe-chat/bipe-shared) | Texts, rules, design tokens, the API contract and test vectors that the other repos generate code from | JSON, Node |
| [bipe-api](https://github.com/bipe-chat/bipe-api) | Sign-up, invites, the @ directory and CNPJ checks | TypeScript, Postgres |
| [bipe-web](https://github.com/bipe-chat/bipe-web) | The site, bipe.chat | TypeScript, Vite |

- Issues labelled [good first issue](https://github.com/search?q=org%3Abipe-chat+label%3A%22good+first+issue%22+state%3Aopen&type=issues) are small and have the file and the fix named in the issue.
- Issues labelled [help wanted](https://github.com/search?q=org%3Abipe-chat+label%3A%22help+wanted%22+state%3Aopen&type=issues) are bigger. Comment on the issue before you start, so two people do not do the same work.
- You can also help without code. Install the test build, use it, and open an issue for each bug. iPhone: [TestFlight](https://testflight.apple.com/join/ehut297S). Android: the test APK at [bipe.chat/baixar](https://bipe.chat/baixar/). Sign-up needs an invite: ask for one in an issue on [bipe-app](https://github.com/bipe-chat/bipe-app/issues).

## Where issues go

Open issues in the public repo that the change touches. If you do not know which repo, use bipe-app.

The team keeps its own task tracker and the design records (ADRs) in a private repo. Some links in the code and in `AGENTS.md` point there and show "404" to you. If you need a decision that a link hides, ask in the issue and we answer there.

## Before you start

- For anything bigger than a small fix, open an issue first. Say what you want to change and why. Bipe keeps a small core on purpose, so some good ideas will wait.
- Each repo has an `AGENTS.md` with its commands, rules and checks. Read it before you open a pull request. The same file guides people and AI agents.
- bipe-shared comes first. A text, a rule or a token that the app, the API and the site share changes in bipe-shared, and the other repos regenerate from it. Do not edit generated files by hand.

## bipe-app: no Element code

bipe-app is written from scratch on matrix-rust-sdk. It must never contain code from Element X (element-hq) or from the archived forks bipe-ios and bipe-android.

- Do not copy, translate or adapt code from those projects into bipe-app.
- matrix-rust-sdk (Apache-2.0), the Matrix spec, and Apple and Android platform docs are fine to read and use.
- If you are not sure that a source is allowed, ask in the issue first.

## AI tools

Most of Bipe's code so far was written by one person working with AI agents. You may use AI tools too. You answer for every line you submit: read it, run the repo's checks, and say in the pull request which parts an AI tool wrote. Human review of any part of Bipe is welcome.

## Sign off your commits (DCO)

Bipe uses the [Developer Certificate of Origin](https://developercertificate.org/). Each commit must end with a sign-off line:

```
Signed-off-by: Your Name <you@example.com>
```

`git commit -s` adds it. The line says that you wrote the change, or have the right to submit it, under the repo's licence. There is no separate agreement to sign.

## Licence

Your contribution to a Bipe repo is licensed under AGPL-3.0-only with the [app store permission](APP-STORE-PERMISSION.md). The permission lets Bipe and anyone else ship the code through app stores such as the Apple App Store.

The archived forks bipe-ios and bipe-android accept no contributions. They hold the source of the current store builds until bipe-app replaces them.

The DCO sign-off confirms that you have the right to license your change on these terms.

## Security

Do not report security problems in public issues. See [SECURITY.md](SECURITY.md).

## Conduct

See [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).
