# kefico-cpegd-seedkey-proof

This repository contains a single cryptographic commitment: a SHA-256 hash
of a working seed/key generation implementation for the UDS SecurityAccess
(diagnostic service 0x27) unlock used on a Kefico CPEGD2.20.x automotive
ECU.

## What this is

A hash, published now, that lets me prove later — without revealing
anything today — that I already had a working implementation as of this
commit's date. This is sometimes called a "commit-reveal" scheme: publish
`hash(x)` first, publish `x` later, and anyone can check that the later `x`
hashes to the same value.

No algorithm, no constants, and no source code are in this repository.
Just the hash and a note of what it covers. See
[`PROOF_2026-07-30_seedkey_algo_sha256.md`](./PROOF_2026-07-30_seedkey_algo_sha256.md).

## Why do it this way

I don't want to publish the implementation yet, but I do want a
verifiable, timestamped record that it already existed at this point, in
case that matters later (for example, establishing priority or
authenticity if I share details in the future). Publishing only the hash
lets me do that without tipping my hand on the actual method.
