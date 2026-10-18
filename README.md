# Windows Package Manager Community Repository

[![Upstream validation](https://img.shields.io/endpoint?url=https://winget-validation-pme-f8gqfjhzacawbecy.z01.azurefd.net/api/GetServiceComponentStatusBadge?component=ValidationPipeline)](https://dev.azure.com/shine-oss/winget-pkgs/_build?definitionId=14)
[![Upstream publishing](https://img.shields.io/endpoint?url=https://winget-validation-pme-f8gqfjhzacawbecy.z01.azurefd.net/api/GetServiceComponentStatusBadge?component=PublishPipeline)](https://dev.azure.com/shine-oss/winget-pkgs/_build?definitionId=12)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

[Deutsch](#deutsch) · [English](#english)

## Deutsch

Dieses Repository ist mein Fork von [microsoft/winget-pkgs](https://github.com/microsoft/winget-pkgs). Das ursprüngliche Projekt enthält die Paketmanifeste für die Standardquelle des Windows Package Managers. Den eigentlichen Kommandozeilen-Client findest du in [microsoft/winget-cli](https://github.com/microsoft/winget-cli).

Ich nutze den Fork für Veyon-Updates über meinen [Veyon → WinGet Bot](https://github.com/Railsimulatornet/veyon-winget-bot). Die Statusanzeigen oben gehören zu den Validierungs- und Veröffentlichungsdiensten des Microsoft-Projekts.

### Inhalt und Aufbau

| Bereich | Inhalt |
| --- | --- |
| [manifests/](manifests/) | Manifeste der Paketversionen |
| [doc/](doc/README.md) | Anleitungen zum Erstellen, Prüfen und Einreichen von Manifesten |
| [schemas/](schemas/) | Schemata für die Manifestprüfung |
| [Tools/](Tools/) | Hilfswerkzeuge für die Arbeit an Manifesten |
| [CONTRIBUTING.md](CONTRIBUTING.md) | Hinweise für Beiträge zum ursprünglichen Projekt |

### Hinweise zu diesem Fork

Der Branch `master` bleibt für die Synchronisierung mit Microsoft reserviert. Mein Veyon-Bot bricht ab, wenn dieser Branch eigene zusätzliche Commits enthält. Diese zweisprachige README wird deshalb auf einem eigenen Dokumentationszweig gepflegt. Änderungen an Manifesten erfolgen ebenfalls auf eigenen Arbeitszweigen.

Ein Pull Request in diesem Fork veröffentlicht noch kein Paket in der offiziellen WinGet-Quelle. Dafür muss die Änderung im Microsoft-Repository geprüft und übernommen werden.

### Unterstützte Pakete

Die Community-Quelle nimmt Anwendungsinstaller in den Formaten MSIX, MSI, APPX, MSIXBundle, APPXBundle und EXE an. Skriptbasierte Installer werden derzeit nicht unterstützt.

Schriftdateien in den Formaten TTF, TTC, OTF, OTC und FNT werden technisch unterstützt. Neue Schriftbeiträge aus der Community werden laut der aktuellen Upstream-Dokumentation jedoch noch nicht angenommen. Prüfe vor einem Beitrag den aktuellen Stand im [Microsoft-Repository](https://github.com/microsoft/winget-pkgs).

### Schnellstart für Beiträge

1. Lies die [Checkliste für den ersten Beitrag](doc/FirstContribution.md).
2. Erstelle oder aktualisiere das Manifest anhand der [Anleitung](doc/README.md#authoring-a-manifest).
3. [Prüfe das Manifest und die Installation](doc/README.md#testing-a-manifest).
4. [Reiche den Pull Request beim Upstream-Projekt ein](doc/README.md#submitting-a-manifest).

Jeder Manifest-PR sollte sich auf ein Paket beziehen. Allgemeine Dokumentationsänderungen gehören in einen getrennten PR.

### Dokumentation und Anfragen

| Thema | Verweis |
| --- | --- |
| Übersicht | [Dokumentation](doc/README.md) |
| Neues Paket anfragen | [Request a New Package](doc/Issues.md#request-a-new-package) |
| Neue Paketversion anfragen | [Request a New Package Version](doc/Issues.md#request-a-new-package-version) |
| Eigene Paketquellen | [Private repositories](doc/private/README.md) |

Die verlinkten Detailanleitungen und Schemaunterlagen stammen aus dem ursprünglichen Projekt und werden dort überwiegend auf Englisch gepflegt.

### Beiträge und Lizenz

Für Beiträge bei Microsoft kann eine Contributor License Agreement (CLA) erforderlich sein. Der CLA-Bot zeigt dies im jeweiligen Pull Request an. Einzelheiten stehen in [CONTRIBUTING.md](CONTRIBUTING.md) und auf [Microsofts CLA-Seite](https://cla.opensource.microsoft.com).

Beachte den [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/) und die zugehörigen [FAQ](https://opensource.microsoft.com/codeofconduct/faq/). Beiträge und verlinkte Inhalte dürfen keine Rechte Dritter verletzen oder entgegen deren Bedingungen eingereicht werden.

Das Repository steht unter der [MIT License](LICENSE). Die ursprünglichen Lizenz- und Urheberhinweise von Microsoft bleiben erhalten.

## English

This repository is my fork of [microsoft/winget-pkgs](https://github.com/microsoft/winget-pkgs). The original project contains package manifests for the Windows Package Manager's default source. The command-line client itself is maintained in [microsoft/winget-cli](https://github.com/microsoft/winget-cli).

I use this fork for Veyon updates through my [Veyon → WinGet Bot](https://github.com/Railsimulatornet/veyon-winget-bot). The badges above show the status of the Microsoft project's validation and publishing services.

### Contents and structure

| Area | Contents |
| --- | --- |
| [manifests/](manifests/) | Manifests for package versions |
| [doc/](doc/README.md) | Instructions for creating, testing and submitting manifests |
| [schemas/](schemas/) | Schemas used to validate manifests |
| [Tools/](Tools/) | Tools for working on manifests |
| [CONTRIBUTING.md](CONTRIBUTING.md) | Contribution guidance for the original project |

### Notes about this fork

The `master` branch is reserved for synchronization with Microsoft. My Veyon bot stops if that branch contains additional commits of its own. This bilingual README is therefore maintained on a separate documentation branch. Manifest changes also use separate working branches.

A pull request in this fork does not publish a package to the official WinGet source. Microsoft must review and merge the change in the upstream repository first.

### Supported packages

The community source accepts application installers in MSIX, MSI, APPX, MSIXBundle, APPXBundle and EXE formats. Script-based installers are not currently supported.

Font files in TTF, TTC, OTF, OTC and FNT formats are technically supported. However, the current upstream documentation states that community font submissions are not yet being accepted. Check the [Microsoft repository](https://github.com/microsoft/winget-pkgs) for the current policy before contributing.

### Contribution quickstart

1. Read the [first-time contributor checklist](doc/FirstContribution.md).
2. Create or update the manifest using the [authoring guide](doc/README.md#authoring-a-manifest).
3. [Test the manifest and installation](doc/README.md#testing-a-manifest).
4. [Submit the pull request to the upstream project](doc/README.md#submitting-a-manifest).

Each manifest PR should cover one package. Keep general documentation changes in a separate PR.

### Documentation and requests

| Topic | Reference |
| --- | --- |
| Overview | [Documentation](doc/README.md) |
| Request a new package | [Request a New Package](doc/Issues.md#request-a-new-package) |
| Request a new package version | [Request a New Package Version](doc/Issues.md#request-a-new-package-version) |
| Host a private package source | [Private repositories](doc/private/README.md) |

The linked detailed guides and schema documentation come from the original project and are mainly maintained in English.

### Contributing and license

Contributions to Microsoft may require a Contributor License Agreement (CLA). The CLA bot reports this in the relevant pull request. See [CONTRIBUTING.md](CONTRIBUTING.md) and [Microsoft's CLA page](https://cla.opensource.microsoft.com) for details.

Follow the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/) and its [FAQ](https://opensource.microsoft.com/codeofconduct/faq/). Contributions and linked materials must respect third-party rights and must not be submitted against the applicable third party's terms.

This repository uses the [MIT License](LICENSE). Microsoft's original license and attribution are preserved.
