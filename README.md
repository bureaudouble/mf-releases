# mf releases

Published builds of [mf](https://github.com/bureaudouble/mf) (its source is private). Nothing is
built here and no workflow runs here: the release workflow of the source repository builds each
version once and uploads the same files to both places.

Each release holds:

- `mf-x86_64-unknown-linux-musl.tar.gz`: the Linux CLI and machine agent (static);
- `mf-aarch64-apple-darwin.tar.gz`: the macOS (Apple Silicon) CLI;
- `install.sh`: the installer machines and laptops run;
- `SHA256SUMS` and `SHA256SUMS.sig`: the checksums, signed by mf's release key.

Install the latest:

```sh
curl -fsSL https://github.com/bureaudouble/mf-releases/releases/latest/download/install.sh | sh
```
