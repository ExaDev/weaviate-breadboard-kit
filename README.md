# A Breadboard Kit for Weaviate

This is a kit to use weaviate with [breadboard](https://github.com/breadboard-ai/breadboard/)

This kit is a an early prototype, and is very likely to change

# Installation

Run the following command to install the kit:

```bash
npm install weaviate-breadboard-kit
```

# Contributing

Update the necessary credentials in [`devcontainer.json`](.devcontainer/devcontainer.json) e.g. PaLM API key, and then rebuild the devcontainer.

# Making a new release

Run the following command to create a new release:

```bash
# Create a new branch
git checkout -b version-bump

# Bump the version
npm version patch -m "Upgrade to %s for reasons"

# Push the branch
git push origin version-bump

# Create a PR to merge the branch into main

# After PR is merged into main, checkout main and pull latest changes
git checkout main
git pull origin main

# Now push the tags, which will trigger the release workflow
git push origin --tags
```