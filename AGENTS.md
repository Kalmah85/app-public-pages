# AGENTS.md

## Project goal

Maintain a generic public repository for static pages associated with applications and projects whose source repositories may remain private.

Primary content includes:
- privacy policies;
- terms of use;
- app/store information pages;
- static informational pages required by external platforms;
- static assets intentionally meant for public distribution.

This repository does not contain application source code.

No individual application is the default scope of this project. Application-specific facts, assumptions and workflows apply only to the relevant page or task and must not become project-wide defaults.

## Public repository rule

Everything committed to this repository must be treated as public.

Never commit:
- passwords, tokens or credentials;
- `.env` files;
- private keys or certificates;
- proprietary source code copied from private repositories;
- internal infrastructure details that are not required for the public pages;
- personal information unless explicitly approved for publication.

## Application-specific content

Privacy policies and similar declarations must describe the verified behavior of the relevant application.

Do not infer or invent:
- collected data;
- shared data;
- permissions;
- SDK behavior;
- analytics;
- advertising;
- retention;
- deletion mechanisms;
- store requirements.

When necessary, inspect the current source repository of the relevant application read-only to verify its behavior.

Do not modify another application's repository from this project unless the user explicitly switches scope and authorizes that work.

## External requirements

When a page exists to satisfy requirements from Google Play or another platform, verify the current external requirements when materially relevant.

Repository documentation or old project state must not override current platform requirements.

## Site layout

The intended GitHub Pages source is:

`docs/`

Application-specific pages should normally follow:

`docs/apps/<app-slug>/privacy/index.html`

`docs/apps/<app-slug>/terms/index.html`

The expected GitHub Pages base URL is:

`https://kalmah85.github.io/app-public-pages/`

Do not assume Pages is deployed or reachable until verified live.

## Development workflow

Before changing repository content:

1. inspect the minimum relevant current state;
2. make the smallest useful change;
3. validate locally;
4. review the diff;
5. stop before consequential actions unless explicitly authorized.

For operational work proceed one block at a time using:

1. Obiettivo
2. Comandi
3. Verifica attesa
4. Stop / fallback

## Authorization

Do not perform consequential operations without explicit user authorization.

This includes:
- commit;
- push;
- merge;
- tag;
- release;
- GitHub Pages publication or configuration;
- changes to another repository.

Authorization applies only to the explicitly approved operation and scope.

## AI Development Platform

Do not assume this repository is authorized for READONLY or DEVELOPMENT execution on the shared AI Development Platform.

Platform eligibility, routing, workers, execution contracts and shared platform governance belong to the global AI Development Platform / OpenCode project and must be verified there when relevant.

## Project State

The Project State is a continuity checkpoint, not a source of truth.

Keep it focused on repository-wide state: repository and branch, canonical checkout, GitHub Pages configuration and verified public URLs, currently published pages, completed milestones, current stop point and next safe step.

Do not turn application-specific implementation details into project-wide assumptions.

## Validation

For published pages, successful validation requires verification of the actual public HTTPS URL.

A Git commit, GitHub branch or Pages configuration alone does not prove that the intended content is publicly available.
