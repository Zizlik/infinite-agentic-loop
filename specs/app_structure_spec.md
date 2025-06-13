# Application Folder Structure Specification

## Purpose
Define the directory and file layout for a complete multi-file application. This specification is language agnostic so it can be adapted to different tech stacks.

## Base Directories
- **src/** - All application source code
  - **components/** - Reusable modules or classes
  - **utils/** - Shared helper functions
- **tests/** - Automated test suites
- **public/** - Static assets served directly to the client
- **docs/** - Project documentation and design notes
- **build/** - Compiled or bundled output

## Required Files
- `README.md` explaining how to run and build the app
- `LICENSE` file specifying project license
- `package.json` or `pyproject.toml` describing dependencies (choose appropriate for stack)
- Configuration files such as `.gitignore` and linting/formatting configs

## File Generation Rules
1. Each directory must contain at least one placeholder file if no real content exists yet.
2. Testing code goes exclusively under `tests/`.
3. Production source files reside only in `src/` and its subfolders.
4. Design documents and diagrams live in `docs/`.
5. Compiled assets are written to `build/` and should not be committed.

Use this structure when generating a new project so all agents know where to place their output.
