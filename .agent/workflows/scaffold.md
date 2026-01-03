---
description: Generate production-ready project structures, components, and boilerplate code
---

# /scaffold <type> <name> [--framework react|vue|angular] [--features hooks,tests,docker,auth]

## Usage Examples

```bash
/scaffold react-component UserProfile --hooks --tests
/scaffold next-app my-project --features auth,docker
/scaffold express-api backend --features tests,auth
```

## Process

1. **Requirements Analysis**
   - Determine target type: react-component, next-app, express-api, fastapi, cli-app
   - Identify framework and features needed

2. **Architecture Planning**
   - Create optimal project structure
   - Configure build and development tools
   - Set up testing infrastructure

3. **Code Generation**
   Generate complete project including:
   - Source code with proper patterns
   - Configuration files (tsconfig, eslint, prettier)
   - Testing setup (jest, vitest, pytest)
   - Docker and CI/CD configuration
   - Documentation and README

## Supported Types

| Type | Description |
|------|-------------|
| `react-component` | React component with hooks, tests, stories |
| `next-app` | Next.js application with API routes |
| `express-api` | Express.js REST API with middleware |
| `fastapi` | Python FastAPI with OpenAPI docs |
| `cli-app` | Node.js or Go CLI application |

## Features

- `--hooks`: Add React hooks
- `--tests`: Include test infrastructure
- `--docker`: Add Docker configuration
- `--auth`: Include authentication setup
- `--ci`: Add CI/CD pipelines
- `--docs`: Generate documentation

## Output Structure

```
project-name/
├── src/
│   ├── components/
│   ├── hooks/
│   ├── services/
│   └── utils/
├── tests/
├── docs/
├── docker/
└── README.md
```
