# Ryan Merrill public key

This repository publishes the public key associated with the GitHub account
[`ryanmerrillmba`](https://github.com/ryanmerrillmba).

## Files

- `archive-mldsa87-public.pem` — the public key in PEM format.
- `archive-mldsa87-public.pem.sha256` — the SHA-256 checksum for the PEM file.
- `archive-mldsa87-public.pem.ots` — the OpenTimestamps proof for the PEM file.

## Verify the public key

Use the checksum file to confirm you have the exact published PEM bytes:

**SHA-256 (`archive-mldsa87-public.pem`):**

```text
4faaa07940542d68f941d0c3e9a6133b5f1c6fd947a1dd5f8bfb275daee8aa13
```

```sh
sha256sum -c archive-mldsa87-public.pem.sha256
```

On macOS, you can compare the displayed value from the following command with
the value in `archive-mldsa87-public.pem.sha256`:

```sh
shasum -a 256 archive-mldsa87-public.pem
```

## Verify the timestamp proof

No software installation is required. Use the official
[OpenTimestamps Stamp & Verify page](https://opentimestamps.org/):

1. In the **Stamp & Verify** section, upload
   `archive-mldsa87-public.pem.ots` as the `.ots proof file to verify`.
2. When prompted, upload the original
   `archive-mldsa87-public.pem` file as the `stamped file`.
3. Review the resulting timestamp and attestation information.

OpenTimestamps calculates the file hash in the browser. A successful
verification shows evidence that the exact PEM file existed no later than the
time anchored by the proof.

The repository's commit history records when these files were published here.
