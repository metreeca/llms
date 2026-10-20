# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres
to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased](https://github.com/metreeca/llms/compare/v0.3.1...HEAD)

## [0.3.1](https://github.com/metreeca/llms/compare/v0.3.0...v0.3.1) - 2026-10-20

### Changed

- `@metreeca/llms-google` — require `@google/genai` `^2.28.0`, so that a consumer on a current SDK release resolves a
  single copy of it and shares its response types with the client, rather than type-checking against a second copy

## [0.3.0](https://github.com/metreeca/llms/compare/v0.2.0...v0.3.0) - 2026-10-20

### Added

- `@metreeca/llms` — embedding vector primitives: `synopsis()` builds the text to be embedded for a resource, `cosine()`
  ranks vectors by semantic proximity, and `compress()`/`decompress()` store them compactly as text
- `@metreeca/llms-google` — `createGoogleAI()` Gemini API client paced against the published rate quotas, honouring
  response schemas alongside tools, with `text()`, `json()` and `embedding()` response accessors
- `@metreeca/llms-openai` — `createOpenAI()` OpenAI API client paced against the published rate quotas, with `text()`,
  `json()` and `embedding()` accessors rejecting refused, truncated and malformed generations

### Changed

- Rename `@metreeca/muse`, `@metreeca/muse-google` and `@metreeca/muse-openai` to `@metreeca/llms`,
  `@metreeca/llms-google` and `@metreeca/llms-openai`; the former names receive no further releases
- Upgrade `@metreeca/core` to `^0.13.0`
- Upgrade `@metreeca/tape` to `^0.12.0`
- Drop the `@metreeca/flow` and `@metreeca/gear` dependencies, which no package imports

## [0.2.0](https://github.com/metreeca/llms/compare/v0.1.1...v0.2.0) - 2026-10-14

### Added

- `@metreeca/muse-openai` — OpenAI model connectors; the module carries no public API yet

### Changed

- Require `@metreeca/core` `^0.12.1`, `@metreeca/flow` `^0.11.1`, `@metreeca/gear` `^0.3.1` and `@metreeca/tape`
  `^0.11.1`, so that a consumer on the current line resolves one copy of each rather than a second, superseded one

## [0.1.1](https://github.com/metreeca/llms/compare/v0.1.0...v0.1.1) - 2026-09-09

### Changed

- requires `@metreeca/core` `^0.10.0`, `@metreeca/flow` `^0.10.0`, `@metreeca/gear` `^0.2.0` and `@metreeca/tape`
  `^0.10.1`, so that a consumer on the current line resolves one copy of each rather than a second, superseded one

## [0.1.0](https://github.com/metreeca/llms/releases/tag/v0.1.0) - 2026-09-04

Initial release, claiming the package names and enabling automated publishing. The modules carry no public API yet:
jobs run under the [@metreeca/gear](https://github.com/metreeca/gear) executor, to which this repository contributes
model services and tasks.

- `@metreeca/muse` — AI tasks and shared services
- `@metreeca/muse-google` — Google model connectors
