# Repository Guidelines

## Project Structure & Module Organization

This repository is currently minimal. `README.md` is the GitHub profile README and is the only project document tracked at the root. Keep root-level files limited to repository-wide documentation and configuration.

If code is added later, place source files in `src/`, static or media assets in `assets/`, and tests in `tests/` or next to the source files they cover. Use clear directory names so future contributors can identify project purpose without guessing.

## Build, Test, and Development Commands

No automated build, test, or development scripts are defined yet. Do not assume commands exist until the required configuration files are added.

- `git status`: check local changes before editing or committing.
- `pnpm install`: install JavaScript dependencies only after a `package.json` exists.
- `pnpm test`: run tests only after a test script is defined in `package.json`.

When adding tooling, document the exact command here in the same change.

## Coding Style & Naming Conventions

Keep Markdown concise, scannable, and specific. Use sentence-case headings, short paragraphs, and relative links for files within the repository. Prefer lowercase kebab-case for new file and directory names, such as `project-notes.md` or `profile-assets/`.

For future code, follow the formatter and linter configured in the project. If none exists, add formatting rules before introducing broad style changes.

## Testing Guidelines

There is no test framework or coverage requirement yet. When tests are introduced, include the framework configuration, a runnable `pnpm test` script, and a short note explaining what the tests cover.

Name test files consistently, for example `*.test.ts`, `*.spec.ts`, or a documented equivalent. Keep tests close to the behavior they validate.

## Commit & Pull Request Guidelines

The current history contains only `Initial commit`, so no detailed convention is established. Use short, imperative commit messages such as `Add profile README guidance`.

Pull requests should include a summary, the reason for the change, and any manual verification performed. For visual changes to the profile README, include screenshots or a preview link when available.

## Agent-Specific Instructions

Always use `pnpm` for JavaScript tooling. Do not use `npm` or `yarn` for installs, scripts, or lockfile updates.
