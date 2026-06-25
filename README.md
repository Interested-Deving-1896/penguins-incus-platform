[update-readmes]   Mode: rewrite — migrating to template structure...
# penguins-incus-platform

[![Built with Ona](https://ona.com/build-with-ona.svg)](https://app.ona.com/#https://github.com/Interested-Deving-1896/penguins-incus-platform)

<!-- AI:start:what-it-does -->
This project provides a unified platform for managing Incus containers and virtual machines within the Penguins ecosystem. It offers a consistent user experience across a Qt6/QML desktop application, a web interface, and a command-line interface, ensuring full feature parity. It is designed for developers and system administrators who require streamlined container and VM management with integrated tooling and workflows.
<!-- AI:end:what-it-does -->

## Architecture

<!-- AI:start:architecture -->
The Penguins Incus Platform consists of three primary components: a Qt6/QML-based desktop UI, a web UI, and a CLI. These components provide unified management for Incus containers and VMs, ensuring feature parity across interfaces. The platform interacts with Incus APIs to manage container and VM lifecycles, networking, and storage. It also integrates with Penguins ecosystem tools for seamless operation.

The repository is organized as follows:

```plaintext
.
├── .devcontainer/          # Development container configuration
├── .github/                # GitHub workflows and CI/CD pipelines
├── config/                 # Configuration files for the platform
├── distrobuilder/          # Tools for building container and VM images
├── integration/            # Integration tests and related scripts
├── oci-builder/            # OCI-compliant image builder
├── penguins-incus-platform/ # Core platform codebase
├── scripts/                # Utility and helper scripts
├── unified-image-server/   # Server for managing unified images
├── ARCHITECTURE.md         # Detailed architecture documentation
├── LICENSE                 # Licensing information
├── README.md               # Project overview and usage instructions
```

The `.github` directory contains workflows for repository automation, including synchronization, artifact mirroring, and CI tasks. Each workflow is defined in YAML files, such as `mirror-orgs-full.yml` and `sync-to-gitlab.yml`.
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
- **add-mirror-repo.yml**: Adds a new repository to the mirror list. Requires `GITHUB_TOKEN` and `MIRROR_API_KEY`.
- **check-gitlab-sync.yml**: Verifies synchronization status between GitHub and GitLab. Requires `GITLAB_TOKEN`.
- **cleanup-pollution.yml**: Removes unused branches and artifacts. Requires `GITHUB_TOKEN`.
- **clone-org.yml**: Clones all repositories from a GitHub organization. Requires `GITHUB_TOKEN`.
- **create-readmes.yml**: Generates README files for repositories. No secrets required.
- **mirror-artifacts.yml**: Syncs build artifacts to external storage. Requires `STORAGE_API_KEY`.
- **mirror-orgs-full.yml**: Mirrors all repositories from specified organizations. Requires `GITHUB_TOKEN` and `MIRROR_API_KEY`.
- **mirror-orgs-watchdog.yml**: Monitors and reports on the health of organization mirrors. Requires `GITHUB_TOKEN`.
- **pr-automation.yml**: Automates pull request labeling and merging. Requires `GITHUB_TOKEN`.
- **rate-limit-status.yml**: Checks and reports API rate limits. Requires `GITHUB_TOKEN`.
- **sync-forks.yml**: Updates forks to match upstream repositories. Requires `GITHUB_TOKEN`.
- **sync-to-gitlab.yml**: Mirrors repositories from GitHub to GitLab. Requires `GITLAB_TOKEN`.
- **token-health.yml**: Validates the health of API tokens. Requires `GITHUB_TOKEN` and `GITLAB_TOKEN`.
- **update-readmes.yml**: Updates README files with the latest information. No secrets required.
- **upstream-prs.yml**: Tracks and syncs upstream pull requests. Requires `GITHUB_TOKEN`.
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
[@Interested-Deving-1896](https://github.com/Interested-Deving-1896): 209 commits

*Note: This repository is a mirror. Please refer to the upstream source for additional contributions and context.*
<!-- AI:end:contributors -->

## Origins

<!-- AI:start:origins -->
_Original project — no upstream fork._
<!-- AI:end:origins -->

## Resources

<!-- AI:start:resources -->
_No additional resource files found._
<!-- AI:end:resources -->

## License

<!-- AI:start:license -->
[GPL-3.0](https://github.com/Interested-Deving-1896/penguins-incus-platform/blob/main/LICENSE) © 2026 [Interested-Deving-1896](https://github.com/Interested-Deving-1896)
<!-- AI:end:license -->
