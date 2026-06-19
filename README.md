# Git-Annoy

A GitHub Actions workflow tool that automatically generates commits to maintain active contribution streaks.

## Overview

Git-Annoy uses scheduled workflows to automatically create commits at configurable intervals, keeping your GitHub contribution graph active without manual effort.

## Features

- **Automated Commits**: Scheduled hourly commits via GitHub Actions
- **Configurable Frequency**: Control commit count per cycle using secrets
- **Weekly History Squashing**: Automatically squashes commits every Sunday
- **Multi-user Support**: Extensible for multiple user configurations
- **Lightweight**: Minimal resource usage with cron-based scheduling

## How It Works

- `commit.yml`: Runs hourly, creates commits and updates commit counters
- `weekly_squash.yml`: Runs weekly, squashes all history into a single commit

## Configuration

Set these GitHub secrets in your repository:

- `USERNAME`: Git user name
- `EMAIL`: Git user email
- `FREQUENCY`: Number of commits per cycle
- `GITHUB_TOKEN`: Personal access token (auto-provided)

## License

MIT
