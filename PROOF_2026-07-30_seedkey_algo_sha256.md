# Prior-Existence Proof — Seed/Key Algorithm (Commit-Reveal, Hash Only)

Date: 2026-07-30

This is a commit-reveal proof of prior existence for a UDS SecurityAccess
(service 0x27) seed/key generation implementation for a Kefico CPEGD2.20.x
ECU. It publishes only a SHA-256 hash of the implementation file — **not the
source itself** — so that the source can be disclosed later and
independently verified against this hash.

## What is hashed

- File: `seedkey_poc.py` (kept private; not included in this repo)
- SHA-256: `1c7805a39820370264b0a9097191cf63fea4a46f576425fadb08a8adfe40ca8a`

## Independent verification

Once (or if) the source is disclosed, anyone can verify it matches this
prior commitment by running:

```
sha256sum seedkey_poc.py
```

The result should match the hash above exactly.

## Not included

No algorithm, no constants, no derivation detail, and no source code are
published in this repo. Only the hash above and the file name it covers.
