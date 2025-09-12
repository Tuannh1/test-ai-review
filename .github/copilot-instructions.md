# Copilot Coding Agent Onboarding Instructions

## High Level Details

**Repository Purpose:**  
This repository implements the "mcp-me" project. It is designed for managing user profiles and authentication for a web application.  
**Project Type:**  
- Web application
- Typical repo size: ~100 files, ~10,000 LOC

**Languages & Frameworks:**  
- Primary language(s): TypeScript, JavaScript
- Frameworks: React, Express
- Target runtime: Node.js v18+

## Build & Validation Instructions

**Environment Setup:**  
- Always run `npm install` before building or testing.
- Node.js projects: Use Node.js v18+ (validate with `node -v`).

**Bootstrap:**  
- If applicable, run `npm run bootstrap` to set up monorepo dependencies.

**Build:**  
- Run `npm run build`.
- If build fails, ensure dependencies are installed and environment variables are set.

**Test:**  
- Run `npm test`.
- Always build before testing.
- Some tests may require a running database or service; check `.env.example` for required environment variables.

**Lint:**  
- Run `npm run lint`.
- Fix lint errors before committing.

**Run:**  
- Use `npm start` to run the application locally.

**Validation Steps:**  
- Ensure all tests pass before submitting changes.
- Check for CI status in GitHub Actions (see `.github/workflows/`).
- If CI fails due to missing dependencies or environment variables, review setup steps above.

**Common Issues & Workarounds:**  
- If build/test fails after a fresh clone, delete `node_modules` and reinstall dependencies.
- For monorepos: Always run bootstrap before build/test.

## Project Layout & Architecture

**Key Directories & Files:**  
- `src/` — Main source code.
- `tests/` — Test suite.
- `package.json` — Node.js project config.
- `.env.example` — Environment variable template.
- `.github/workflows/` — CI/CD pipelines.
- `README.md` — Project overview and usage.
- `CONTRIBUTING.md` — Contribution guidelines.

**Configuration Files:**  
- Lint: `.eslintrc`
- Build: `tsconfig.json`, `webpack.config.js`
- Test: `jest.config.js`, `pytest.ini`

**Validation Pipelines:**  
- GitHub Actions run on push and pull request.
- Checks: build, lint, test.
- All must pass for PR approval.

**Explicit Validation Steps:**  
- Run build, lint, and test locally before pushing.
- Review CI logs for errors.
- Use provided scripts in `package.json` or equivalent.

**Dependencies:**  
- All dependencies are listed in `package.json`.
- For non-obvious dependencies, check README and setup scripts.

## Repo Root File List

- `README.md`
- `package.json`
- `.env.example`
- `.github/`
- `src/`
- `tests/`

## README & Key Source File Snippets

- See `README.md` for project overview, setup, and usage.
- Main entry point: `src/index.ts`
- Example main method:
  ```typescript
  // src/index.ts
  function main() {
    // ...existing code...
  }
  ```

## Agent Guidance

- Trust these instructions for build, test, and validation steps.
- Only perform additional search if information here is incomplete or incorrect.
- Prioritize using documented commands and file locations.
- Avoid unnecessary exploration; follow the documented workflow for efficiency.
