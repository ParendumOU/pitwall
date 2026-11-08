# Pitwall

Pitwall runs Claude Code across several subscriptions as one: it picks the account with most capacity, moves the same conversation to the next account when a usage limit is reached, switches live or on a schedule, and shows usage and cost on a web dashboard. A Pitwall server keeps the accounts of all your machines in one place, and the Pitwall Remote app follows and drives your sessions from the phone.

## Install

The Pitwall installer sets up Pitwall with everything around it, and keeps it updated:

```bash
curl -fsSL https://github.com/ParendumOU/pitwall-bootstrap/releases/latest/download/install.sh | bash
```

```powershell
irm https://github.com/ParendumOU/pitwall-bootstrap/releases/latest/download/install.ps1 | iex
```

By hand: download `pitwall-<version>.tar.gz` from a release, check it against `SHA256SUMS` (`sha256sum -c SHA256SUMS --ignore-missing`), unpack it and link it (`pnpm add -g .` in its folder, Node.js 18 or newer), then run `pitwall install`.

## More

Website: https://pitwall.parendum.com

License: MIT (see [LICENSE](LICENSE)). Each release includes its full source.
