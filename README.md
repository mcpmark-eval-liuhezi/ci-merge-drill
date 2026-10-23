# ci-merge-drill

Merge-gate demonstration repository for an annual engineering review evidence packet.

## Purpose

This repository demonstrates an end-to-end change-delivery drill: a CI workflow is registered
on push, a branch is cut, a README edit is proposed via pull request, and the change is
squash-merged into the default branch after the CI workflow is confirmed to be registered.

## CI

A minimal continuous integration workflow lives at `.github/workflows/ci.yml`. It triggers
on every push and runs a single job that echoes a confirmation message.
