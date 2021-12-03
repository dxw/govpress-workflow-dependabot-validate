# GovPress Workflow: Dependabot Validate

This repo holds a reusable workflow for validating Dependabot files in GovPress projects.

You can pass it any `package-ecosystem` (e.g. `composer`), and the corresponding filename for that package manager (e.g. `composer.json`). It will search the repo for any files matching that filename, and then check if the `dependabot.yml` file contains an entry for all found files for that package ecosystem. If it does not, the workflow will fail.
