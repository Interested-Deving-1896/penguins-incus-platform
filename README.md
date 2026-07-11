[update-readmes]   Mode: rewrite — migrating to template structure...
# penguins-incus-platform

[![Built with Ona](https://ona.com/build-with-ona.svg)](https://app.ona.com/#https://github.com/Interested-Deving-1896/penguins-incus-platform) [![KDE Eco](https://img.shields.io/badge/KDE%20Eco-certified-brightgreen?logo=kde&logoColor=white&style=flat-square)](https://eco.kde.org/) [![Blue Angel](https://img.shields.io/badge/Blue%20Angel-DE--UZ%20215-0055a4?style=flat-square)](https://www.blauer-engel.de/en/certification/criteria) [![Energy](https://api.green-coding.io/v1/ci/badge/get?repo=Interested-Deving-1896%2Fpenguins-incus-platform&branch=main&workflow=eco-audit.yml)](https://metrics.green-coding.io/ci-index.html)


<!-- AI:start:what-it-does -->
This project provides a unified platform for managing Incus containers and virtual machines within the Penguins ecosystem. It offers a Qt6/QML-based desktop UI, a web UI, and a CLI, ensuring feature parity across all interfaces. It is designed for developers and system administrators who require consistent and streamlined tools for container and VM lifecycle management.
<!-- AI:end:what-it-does -->

## Architecture

<!-- AI:start:architecture -->
The Penguins Incus Platform consists of three primary components: a Qt6/QML-based desktop UI, a web UI, and a CLI. These components provide unified management for Incus containers and VMs within the Penguins ecosystem, ensuring feature parity across interfaces. The platform interacts with Incus APIs for container and VM operations and integrates with additional tools for image building, artifact mirroring, and repository synchronization.

The repository is organized as follows:

```plaintext
penguins-incus-platform/
├── .devcontainer/         # Development container configuration
├── .github/               # GitHub workflows and CI/CD configurations
├── distrobuilder/         # Tools for building Linux distributions
├── integration/           # Integration tests and related scripts
├── oci-builder/           # OCI-compliant image builder
├── scripts/               # Utility scripts for automation and maintenance
├── unified-image-server/  # Server for managing and distributing images
├── ARCHITECTURE.md        # Detailed architecture documentation
├── LICENSE                # License information
├── README.md              # Project overview and usage instructions
```

The `.github` directory contains workflows for repository management, synchronization, and automation tasks. The `scripts` directory includes helper scripts for tasks like token rotation, repository mirroring, and upstream synchronization. Each component is modular to facilitate independent development and deployment.
<!-- AI:end:architecture -->

## Install

<!-- Add installation instructions here. This section is yours — the AI will not modify it. -->

```bash
git clone https://github.com/Interested-Deving-1896/penguins-incus-platform.git
cd penguins-incus-platform
```

## Usage

<!-- Add usage examples here. This section is yours — the AI will not modify it. -->

## Configuration

<!-- Document configuration options here. This section is yours — the AI will not modify it. -->

## CI

<!-- AI:start:ci -->
- **add-mirror-repo.yml**: Adds a new repository to the mirror list. Requires `MIRROR_API_TOKEN`.
- **check-gitlab-sync.yml**: Verifies synchronization status between GitHub and GitLab. Requires `GITLAB_TOKEN`.
- **cleanup-pollution.yml**: Cleans up temporary or polluted branches. No secrets required.
- **clone-org.yml**: Clones all repositories from a specified organization. Requires `GITHUB_TOKEN`.
- **create-readmes.yml**: Generates README files for repositories. No secrets required.
- **fork-neon-repos.yml**: Forks Neon-related repositories. Requires `GITHUB_TOKEN`.
- **gl-storage-scan.yml**: Scans GitLab storage usage. Requires `GITLAB_TOKEN`.
- **import-repo.yml**: Imports repositories into the project. Requires `IMPORT_API_TOKEN`.
- **inject-badges.yml**: Adds badges to README files. No secrets required.
- **mirror-artifacts.yml**: Mirrors build artifacts between platforms. Requires `ARTIFACT_API_TOKEN`.
- **mirror-orgs-full.yml**: Performs a full mirror of all repositories in an organization. Requires `MIRROR_API_TOKEN`.
- **pr-automation.yml**: Automates pull request workflows. Requires `GITHUB_TOKEN`.
- **rate-limit-status.yml**: Monitors API rate limits. Requires `GITHUB_TOKEN`.
- **sync-forks.yml**: Synchronizes forks with upstream repositories. Requires `GITHUB_TOKEN`.
- **update-readmes.yml**: Updates README files across repositories. No secrets required.
<!-- AI:end:ci -->

## Mirror chain

<!-- AI:start:mirror-chain -->
This repo is maintained in [`Interested-Deving-1896/penguins-incus-platform`](https://github.com/Interested-Deving-1896/penguins-incus-platform) and mirrored through:

```
Interested-Deving-1896/penguins-incus-platform  ──►  OpenOS-Project-OSP/penguins-incus-platform  ──►  OpenOS-Project-Ecosystem-OOC/penguins-incus-platform
```

Changes flow downstream automatically via the hourly mirror chain in
[`fork-sync-all`](https://github.com/Interested-Deving-1896/fork-sync-all).
Direct commits to OSP or OOC are detected and opened as PRs back to `Interested-Deving-1896`.
<!-- AI:end:mirror-chain -->

## Contributors

<!-- AI:start:contributors -->
[@Interested-Deving-1896](https://github.com/Interested-Deving-1896): 220 commits

*Note: This repository is a mirror. Please refer to the upstream source for additional contributions and updates.*
<!-- AI:end:contributors -->

## Origins

<!-- AI:start:origins -->
_Original project — no upstream fork._
<!-- AI:end:origins -->

## Resources

<!-- AI:start:resources -->
_No additional resource files found._
<!-- AI:end:resources -->

<!-- AI:start:accessibility -->
This repo uses automated accessibility auditing via `check-accessibility.yml`.

Checks include: CODEOWNERS ownership coverage, README screen-reader compatibility,
WCAG 2.1 AA HTML compliance, audio overview (espeak-ng), and Braille output (liblouis).




Run the [Check Accessibility](https://github.com/Interested-Deving-1896/penguins-incus-platform/actions/workflows/check-accessibility.yml)
workflow to generate the first report and accessibility artifacts.
See [DOCS/accessibility.md](https://github.com/Interested-Deving-1896/penguins-incus-platform/blob/main/DOCS/accessibility.md) for the full reference.
<!-- AI:end:accessibility -->

## License

<!-- AI:start:license -->
[GPL-3.0](https://github.com/Interested-Deving-1896/penguins-incus-platform/blob/main/LICENSE) © 2026 [Interested-Deving-1896](https://github.com/Interested-Deving-1896)
<!-- AI:end:license -->
