# SylphxAI Codec

SylphxAI/codec is a TypeScript/Bun monorepo for universal media codec, image-processing, and conversion packages, with optional WASM acceleration.

## Lifecycle

- State: `active`
- Layer: `foundation`
- Machine manifest: [`.doctrine/project.json`](./.doctrine/project.json)

## Goals

- Provide core media codec and conversion packages for image, video, animation, audio, metadata, drawing, filtering, transforms, compositing, and CLI usage.
- Maintain pure TypeScript codec implementations with optional WASM acceleration where the repository explicitly provides it.
- Track codec coverage, tests, and remaining media-format work through repo-local package code and progress documentation.

## Non-Goals

- This repository does not own application-specific media workflows, storage products, CDN behavior, or user-facing media tools.
- This repository does not own third-party codec patents, platform codec licensing, or external media-processing infrastructure.
- This repository does not own enterprise engineering doctrine.

## Boundary

This repository owns the codec/conversion package monorepo, media format implementations, processing packages, tests, optional WASM backend scaffolding, and release workflow. Consuming applications own their product workflows, media storage, user interfaces, deployment, licensing decisions, and operational policy.

## Public Surfaces

- Root package manifest and scripts: [`package.json`](./package.json)
- Progress and coverage tracker: [`PROGRESS.md`](./PROGRESS.md)
- Core package: [`packages/core/`](./packages/core/)
- Codec package: [`packages/codecs/`](./packages/codecs/)
- CLI package: [`packages/cli/`](./packages/cli/)
- Processing packages: [`packages/transform/`](./packages/transform/), [`packages/color/`](./packages/color/), [`packages/filter/`](./packages/filter/), [`packages/composite/`](./packages/composite/), [`packages/draw/`](./packages/draw/), [`packages/histogram/`](./packages/histogram/), [`packages/metadata/`](./packages/metadata/), [`packages/text/`](./packages/text/)
- WASM package: [`packages/wasm/`](./packages/wasm/)
- Release workflow: [`.github/workflows/release.yml`](./.github/workflows/release.yml)

## Delivery

The repository has a reusable main-branch release workflow but no recorded pull-request CI workflow. Production proof is package tests, build for changed packages, codec fixture validation for affected formats, release workflow evidence, and package-registry readback for published versions. This manifest slice is documentation-only and does not change package code, codec behavior, CI, release, or WASM behavior.
