# Maintenance

CodeQL checks this fork's GitHub Actions workflows when files under `.github/` change and once a week. A targeted checkout keeps the analysis focused on GitHub configuration files.

The existing PowerShell checks continue to validate PowerShell changes. This CodeQL workflow checks only the Actions configuration.
