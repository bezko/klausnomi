# AGENTS.md - klausnomi Project

## Phase 1: Architecture Discovery (1 day)
- Sample directory structure:
  - `core/mcp.py`
  - `commands/chat_commands.py`
  - `auth.py`
  - `utils/logging.py`
- CI/CD config for branch protection

## Phase 2: Python Translation (5 days)
1. Main CLI entry point: `__main__.py`
2. Error handlers with context-aware messages
3. Bulk operation utilities

## Phase 3: Integration (3 days)
- Add type annotations
- Make session management optional
- Add telemetry middleware

## Phase 4: Testing (2 days)
- Create integration tests for chat commands
- Validate configuration changes

## Phase 5: Deployment (1 day)
- Update packaging scripts