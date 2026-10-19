# MedEssist Releases

Public download feed for MedEssist terminal updates. There is no source code
here. Releases are published automatically by CI from the private
MedEssist-Code repo whenever a version is tagged.

Each release carries:

| File | Used by |
|---|---|
| `latest.json` | MedEssist.exe, to find its next update |
| `latest-production.json` | MedEssist-Production.exe, to find its next update |
| `MedEssist-<version>.exe` | the standard build |
| `MedEssist-Production-<version>.exe` | the production build |
| `MedEssist-Setup-<version>.exe`, `MedEssist-Production-Setup-<version>.exe` | first-time installs |

Terminals only install a build whose manifest carries a valid MedEssist
signature, so a file in this repo is not trusted just because it is here.

Do not commit anything to this repo by hand. Do not delete old releases: a
terminal that has fallen behind still downloads the current one, but the
history is the record of what shipped.
