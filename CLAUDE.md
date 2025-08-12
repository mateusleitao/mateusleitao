# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is Mateus Leitão's GitHub profile repository containing:
- A comprehensive README.md with personal information, tech stack, and GitHub analytics
- Automated GitHub contribution snake animation generation via GitHub Actions

## Architecture

- **Profile Repository**: This is a special GitHub repository (username/username) that displays on the GitHub profile page
- **GitHub Actions Workflow**: `.github/workflows/main.yml` automatically generates a snake animation from GitHub contributions every 24 hours
- **Output Branch**: The workflow pushes generated SVG animations to an `output` branch for use in the README

## Key Components

- **README.md**: Main profile display featuring animated headers, tech stack badges, GitHub statistics, and social links
- **Snake Animation**: Generated from GitHub contributions graph using Platane/snk action, available in both light and dark themes
- **Automated Workflow**: Runs on schedule, manual trigger, or pushes to master branch

## Development Notes

- This is primarily a display repository with no build/test/lint commands needed
- Any changes to README.md will be immediately visible on the GitHub profile
- The GitHub Actions workflow requires `GITHUB_TOKEN` permissions for publishing to the output branch
- Snake animation files are auto-generated and should not be manually edited