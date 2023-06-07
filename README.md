# PET Pipeline Repo

This repository holds workflows and pre-commits used by the CSM Platform
Enablement Team (PET).

## How to use a workflow

This repository contains reusable workflows located under .github/workflows. To
use a workflow you can copy the appropriate workflow from the examples/workflows
directory to your repos .github/workflows directory.

## How to use pre-commit actions

Your repo needs a .pre-commit-config.yaml file in it's root directory that
points to the hooks you wish to use. See the pre-commit
[Adding Plugins](https://pre-commit.com/#plugins) page for more information on
how to do this. There are also example files in examples/pre-commit that can be
used.

To use the pre-commits you need to install [pre-commit](https://pre-commit.com/)
using either homebrew or pip.

    brew install pre-commit

OR pip install --user pre-commit

Once this is done you can run the following command to enable pre-commit to run
for the repo you've cloned

    pre-commit install

This will setup the pre-commit hooks to run for that git repo.

There is also a Brewfile available in the hooks directory that can be used to
install the applications required for all hooks in this repo.
