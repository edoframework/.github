# Security policy

## Reporting a vulnerability

Please report security problems privately to **security@taihei.dev**. Do not open a public
issue, pull request or discussion.

Include the library and version, a description of the problem and how it can be exploited, and, if
you can, a minimal reproduction.

## What happens next

- We acknowledge your report within five working days.
- We investigate, keep you informed, and agree on a disclosure date with you.
- We release a fix for every supported version line and publish an advisory on GitHub before the
  details become public. We credit you in the advisory unless you prefer otherwise.

## Supported versions

The latest major version of each library receives security fixes. When a new major version is
released, the previous major version receives security fixes for 12 months after the new one
ships.

## Verifying releases

Every release on Maven Central under `dev.taihei` is signed by
the Taihei Framework release key (UID `Edo Framework Releases <releases@edoframework.com>`,
from before the family was renamed), fingerprint
`5026 B299 6DDB 697E C463  0BCF 14A7 33E2 A507 702F`, published on keyserver.ubuntu.com and
keys.openpgp.org.
