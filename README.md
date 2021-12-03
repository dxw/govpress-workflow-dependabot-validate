# GovPress Workflow: Dependabot Validate

This repo holds a reusable workflow for validating Dependabot files in GovPress projects.

It will search the repo for `composer.json` and `package.json` files, and then check there is an entry for each one in the repo's `dependabot.yml`. If there isn't, the workflow will fail.

This should ensure we don't allow our `dependabot.yml` files to fall out of date by not updating them when we add new `composer.json` or `package.json` files to a repo.
