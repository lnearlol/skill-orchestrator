# Skill Orchestrator

Repository of project-specific skillsets for Claude Code.

## Projects

### TNB
- **Repository**: `tnb-software/TNB`
- **Skillset directory**: `skillsets/TNB`
- **Description**: TNB (Test iN a Box) upstream framework. Contains reusable test components, system-x service connectors, and test templates.

### tnb-tests
- **Repository**: `jboss-fuse-qe/t-n-b/tnb-tests`
- **Skillset directory**: `skillsets/tnb-tests`
- **Description**: Downstream QE test suites built on top of TNB. Contains test configurations, settings, and product-specific test scenarios.

## How it works

The global skill `/install-skillset` detects the current project by extracting the repository name from `git remote get-url origin`, finds the matching skillset directory, and copies the skills into the project's `.claude/commands/`.
