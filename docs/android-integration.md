# Android integration contract

## Public issue forms
- Bug: https://github.com/mojrs10/DeepMox-Support/issues/new?template=bug_report.yml
- Feature: https://github.com/mojrs10/DeepMox-Support/issues/new?template=feature_request.yml
- UI/UX: https://github.com/mojrs10/DeepMox-Support/issues/new?template=ui_feedback.yml
- Question: https://github.com/mojrs10/DeepMox-Support/issues/new?template=question.yml
- All Issues: https://github.com/mojrs10/DeepMox-Support/issues

GitHub sign-in is required to submit an Issue.

## No embedded credentials
The Android app must not contain a GitHub personal access token, App private key, client secret, or any credential capable of creating or modifying repository content. Open browser URLs for write operations. Public read-only API requests may be unauthenticated and are subject to GitHub rate limits.

## Diagnostic handoff
Diagnostics must be opt-in and user-reviewed. Exclude by default:
- Proxmox API tokens, passwords, cookies, and session identifiers.
- Private keys and recovery codes.
- Host IP addresses, DNS names, usernames, and cluster names.
- Terminal output and arbitrary configuration contents.

Show the exact diagnostic text before copying. Never silently upload logs or files.

## Version metadata
Include app version and build number. Android version and device model may be included only after disclosure and user confirmation. Do not collect serial numbers or hardware identifiers.

## Issue list and status
The app may open the public Issues page in a browser. An in-app list may use unauthenticated, read-only GitHub API requests with pagination, caching, and rate-limit handling. Without user authentication or a backend, the app cannot securely provide personalized per-user issue filtering.

Use GitHub Issue state and maintainer-applied labels. Do not infer release dates from planned or in-progress.
