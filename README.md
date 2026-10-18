# R3BL Binary Releases (`r3bl-org/r3bl-binaries`)

Official pre-compiled binary releases for **R3BL** products both closed and open source.

All pre-compiled archives (`.tar.gz` for Linux & macOS, `.zip` for Windows) and `.sha256`
checksums are published as
[GitHub Releases](https://github.com/r3bl-org/r3bl-binaries/releases) in this repository.

---

## Quick Install

### Linux & macOS

```bash
# Install r3bl-cmdr (giti, edi, env-source) - default
curl -LsSf https://r3bl.com/install.sh | sh

# Install specific suite (cmdr | build-infra | mcp-server | all)
curl -LsSf https://r3bl.com/install.sh | sh -s -- all
```

### Windows (PowerShell)

```powershell
# Install r3bl-cmdr (giti, edi, env-source) - default
irm https://r3bl.com/install.ps1 | iex
```

---

## Self-Upgrade

Every R3BL binary includes a built-in `--upgrade` flag that checks
[`https://r3bl.com/versions.json`](https://r3bl.com/versions.json) and upgrades itself
in-place from this repository's releases:

```bash
giti --upgrade
edi --upgrade
env-source --upgrade
cargo-rustdoc-fmt --upgrade
rust-analyzer-mcp-server --upgrade
```

---

## Links

- **Website**: [https://r3bl.com](https://r3bl.com)
- **Version Manifest**: [https://r3bl.com/versions.json](https://r3bl.com/versions.json)
- **Open Core Source Repository**:
  [https://github.com/r3bl-org/r3bl-open-core](https://github.com/r3bl-org/r3bl-open-core)
