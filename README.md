# Ryan Merrill public key

This repository publishes the public key associated with the GitHub account
[`ryanmerrillmba`](https://github.com/ryanmerrillmba).

## Files

- `archive-mldsa87-public.pem` — the public key in PEM format.
- `archive-mldsa87-public.pem.sha256` — the SHA-256 checksum for the PEM file.
- `archive-mldsa87-public.pem.ots` — the OpenTimestamps proof for the PEM file.

## Verify the public key

Use the checksum file to confirm you have the exact published PEM bytes:

```sh
sha256sum -c archive-mldsa87-public.pem.sha256
```

On macOS, you can compare the displayed value from the following command with
the value in `archive-mldsa87-public.pem.sha256`:

```sh
shasum -a 256 archive-mldsa87-public.pem
```

## Verify the timestamp proof

Install [OpenTimestamps](https://opentimestamps.org/) and run:

```sh
ots verify archive-mldsa87-public.pem.ots
```

If the proof needs newer calendar attestations, run `ots upgrade` first and
then verify it again. A successful verification shows evidence that the public
key's exact contents existed no later than the time anchored by the proof.

The repository's commit history records when these files were published here.
