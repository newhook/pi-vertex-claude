# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- Self-healing logic to detect and fix orphaned `tool_use` blocks that are missing corresponding `tool_result` blocks
- Automatic injection of synthetic error tool results when conversation state corruption is detected

### Changed
- Upgraded `@anthropic-ai/sdk` from 0.54.0 to 0.80.0
- Upgraded `@anthropic-ai/vertex-sdk` from 0.11.4 to 0.14.4

### Fixed
- Fixed 400 errors from Vertex AI when tool_use blocks lack corresponding tool_result blocks
- Improved streaming reliability and tool calling stability

## [0.1.3] - 2026-02-07

### Added
- Support for Claude Opus 4.6 model (`claude-opus-4-6`)

## [0.1.2] - 2025-01-30

### Changed
- Further simplified README - removed Features and Common Issues sections
- Cleaner title and structure following Pi extension conventions
- Removed copyright from LICENSE and README

### Removed
- GitHub Actions workflow (tests need peer dependencies)

## [0.1.1] - 2025-01-30

### Changed
- Simplified README - removed unnecessary sections (pricing, fish shell, excessive troubleshooting)
- Cleaner, more focused documentation

## [0.1.0] - 2025-01-30

### Added
- Initial release
- Support for all Vertex AI Claude models (Opus, Sonnet, Haiku)
- Full streaming support
- Extended thinking for reasoning models
- Tool/function calling support
- Image input support
- Prompt caching
- Token usage tracking and cost calculation
- Comprehensive test suite
- NPM and GitHub distribution
