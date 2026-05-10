# Rat Trap Sentinel Public Demo Target

This repository is a safe public fixture for Rat Trap Sentinel demos.

It is not the Sentinel product source code. It exists so the private Sentinel app can scan a stable public GitHub repository and demonstrate:

- branch scans from a public repo,
- pull-request changed-file scans,
- review queue routing,
- evidence exports,
- GitHub handoff dry-run or live issue delivery.

The files are intentionally small and synthetic. Some configuration shapes are unusual on purpose so Sentinel has a repeatable finding to route during demos.

## Demo Flows

Branch scan target:

```text
Martin123132/Rat-Trap-Sentinel-public- @ main
```

Pull-request scan target:

```text
Martin123132/Rat-Trap-Sentinel-public- # permanent demo PR
```

The permanent demo PR is intentionally left open so Sentinel can repeatedly demonstrate PR changed-file scanning. Do not merge or close that PR unless a replacement PR is created and the private Sentinel product defaults are updated first.

Keep secrets, credentials, and real customer code out of this repository.
