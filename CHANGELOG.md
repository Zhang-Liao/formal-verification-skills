# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.1] - 2026-03-07

### Added
- **`/fvs:weekly-summary` command** - Generate weekly progress reports from git commits with AI-powered narrative summaries
  - Analyzes git commits over a configurable time period (default: 7 days)
  - Groups commits by author with detailed context
  - Generates professional narrative summaries using the `fvs-weekly-summary` agent
  - Outputs formatted markdown reports to file or console
  - Includes real-world examples from Dalek-Lean project updates

- **New agent: `fvs-weekly-summary`** - Specialized agent for analyzing git commits and generating professional technical summaries

- **New reference documentation**:
  - `fv-skills/references/weekly-summary-examples.md` - Real-world examples from project updates
  - `fv-skills/workflows/weekly-summary.md` - Detailed workflow documentation

### Changed
- Improved documentation structure with centralized examples in `references/` directory
- Enhanced execution context system for better separation of concerns

### Fixed
- File permissions for weekly-summary related files (changed from 600 to 644)

## [0.1.0] - 2026-02-09

### Added
- Initial release of Formal Verification Skills (FVS)
- Multi-runtime support: Claude Code, OpenCode, and Gemini CLI
- Multi-platform support: Mac, Windows, and Linux

#### Framework-agnostic commands:
- `/fvs:map-code` - Build function dependency graph from extracted code
- `/fvs:plan` - Pick verification targets via dependency graph traversal
- `/fvs:natural-language` - Generate natural language explanations with pre/post conditions
- `/fvs:help` - Command usage guide
- `/fvs:update` - Self-update functionality

#### Lean 4 (via Aeneas) commands:
- `/fvs:lean-specify` - Generate Lean spec skeletons with `@[progress]` theorem pattern
- `/fvs:lean-verify` - Attempt proofs using domain-specific tactics

#### Infrastructure:
- Automated installer with interactive and non-interactive modes
- Custom statusline showing model, current task, and context usage
- Session hooks for update checking
- Comprehensive reference documentation for Lean 4, Aeneas patterns, proof strategies, and tactic usage
- Specialized agents for code analysis, specification generation, and proof attempts

### Documentation
- README with installation instructions and workflow guide
- Reference documentation for Lean 4 conventions, proof strategies, and tactic usage
- UI branding guidelines

[0.1.1]: https://github.com/yourusername/formal-verification-skills/compare/v0.1.0...v0.1.1
[0.1.0]: https://github.com/yourusername/formal-verification-skills/releases/tag/v0.1.0
