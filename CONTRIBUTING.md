# Contributing to the Taihei Framework

Thank you for taking the time to help. The Taihei Framework is a family of open-source Scala 3
libraries, maintained by Innovenso BV and released under the Apache License 2.0.

## Before you start

- **Bugs**: open an issue with a minimal reproduction: the library and version, the Scala version,
  the platform (JVM or Scala.js), what you expected and what happened.
- **Questions**: open an issue; if the answer should have been in the README, we will fix the
  README too.
- **Features**: open an issue to discuss the idea before you write code, so your time is not
  spent on something we cannot take.
- **Security problems**: never open a public issue. See [SECURITY.md](SECURITY.md).

## Building

Every repository builds with Mill from a fresh clone. No credentials are needed, and every
dependency comes from Maven Central.

```sh
make validate      # scalafix, scalafmt, compile and test, on the JVM and Scala.js
make test          # the tests only (Scala.js tests run under Node)
```

You need a JDK (21 or later) and, for Scala.js, Node.js.

## Sending a change

1. Fork the repository and create a branch from `main`.
2. Keep the change focused: one bug or one feature per pull request.
3. Add tests that fail without your change, on both platforms where the library is
   cross-platform.
4. Run `make validate` and make sure it passes.
5. Sign off every commit (see below) and open a pull request against `main`.

A change to a published API follows semantic versioning: a patch fixes, a minor adds, a major
breaks. If your change breaks binary or source compatibility, say so in the pull request; it can
only land in a major release.

## Developer Certificate of Origin

Every commit must be signed off, which certifies that you wrote it or otherwise have the right to
submit it under the project's licence, as described in the
[Developer Certificate of Origin 1.1](https://developercertificate.org/). Add the line with
`git commit -s`:

```
Signed-off-by: Your Name <your.email@example.com>
```

The name and address must match the commit's author. A pull request with unsigned commits cannot be
merged; `git rebase --signoff main` signs off the commits you already made.

## Code of conduct

Everyone who takes part follows the [Code of Conduct](CODE_OF_CONDUCT.md). Report unacceptable
behaviour to hello@taihei.dev.
