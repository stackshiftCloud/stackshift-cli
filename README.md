# StackShift CLI

Signed command-line releases for StackShift.

## Install on macOS or Linux

Install `cosign`, then run:

```sh
curl -fsSLO \
  https://github.com/stackshiftCloud/stackshift-cli/releases/download/v1.0.2/install-cli.sh
chmod 0755 install-cli.sh
STACKSHIFT_CLI_VERSION=v1.0.2 ./install-cli.sh
```

## Install on Windows

Install `cosign`, then run in PowerShell:

```powershell
Invoke-WebRequest `
  https://github.com/stackshiftCloud/stackshift-cli/releases/download/v1.0.2/install-cli.ps1 `
  -OutFile install-cli.ps1
$env:STACKSHIFT_CLI_VERSION = "v1.0.2"
.\install-cli.ps1
```

The installers verify the Sigstore checksum bundle and the selected archive's
SHA-256 digest before installing anything.

Authenticate with:

```sh
stackshift auth login
```
