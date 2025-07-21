# Nx Monorepo Template

A modern, scalable TypeScript monorepo template powered by **Nx** and **Biome.js**.

## 🚀 Features

- **Nx 21.3.1** - Powerful monorepo tooling with intelligent caching and task orchestration
- **TypeScript 5.8+** - Modern TypeScript with strict configuration
- **Biome.js 2.1.2** - Fast linter and formatter (ESLint + Prettier replacement)
- **pnpm** - Fast, disk space efficient package manager
- **Jest** - Testing framework with SWC for fast execution
- **Webpack** - Bundling and development server
- **ESBuild** - Ultra-fast bundler for production builds
- **Express** - Node.js web framework support
- **React** - Frontend framework support with hot reload

## 📦 What's Included

### Core Tools

- **Nx** - Monorepo orchestration and task running
- **Biome.js** - Linting and formatting (configured with accessibility and security rules)
- **TypeScript** - Strict configuration with modern ES2022 target
- **Jest** - Testing with SWC for performance
- **Webpack** - Development and production bundling

### Pre-configured Plugins

- `@nx/js` - JavaScript/TypeScript project support
- `@nx/webpack` - Webpack integration
- `@nx/jest` - Jest testing integration
- `@nx/express` - Express.js applications
- `@nx/web` - Web applications
- `@nx/node` - Node.js applications
- `@nx/esbuild` - ESBuild for fast builds

## 🛠️ Quick Start

### Prerequisites

- Node.js 18+
- pnpm 8+

### Installation

1. **Clone the template**

   ```bash
   git clone <your-repo-url>
   cd nx-mono-repo-template
   ```

2. **Install dependencies**

   ```bash
   pnpm install
   ```

3. **Verify setup**

   ```bash
   # Check code formatting and linting
   pnpm check

   # Fix formatting and linting issues
   pnpm fix
   ```

## 📁 Project Structure

```
nx-mono-repo-template/
├── apps/                    # Applications
│   └── .gitkeep
├── libs/                    # Shared libraries
│   └── .gitkeep
├── biome.jsonc             # Biome.js configuration
├── nx.json                 # Nx workspace configuration
├── package.json            # Root package.json
├── pnpm-workspace.yaml     # pnpm workspace configuration
├── tsconfig.base.json      # Base TypeScript configuration
└── tsconfig.json           # Root TypeScript configuration
```

## 🎯 Available Scripts

### Root Level Scripts

- `pnpm check` - Run Biome.js linting and formatting checks
- `pnpm fix` - Fix formatting and linting issues automatically

### Nx Commands

- `npx nx graph` - Visualize project dependencies
- `npx nx run-many --target=build` - Build all projects
- `npx nx run-many --target=test` - Test all projects
- `npx nx run-many --target=lint` - Lint all projects

## 🔧 Configuration

### Biome.js Configuration

The template includes a comprehensive Biome.js configuration with:

- **Accessibility rules** - WCAG compliance warnings
- **Security rules** - Security best practices
- **Code quality rules** - Maintainable code patterns
- **Formatting** - Consistent code style with tabs, 150 char line width

### TypeScript Configuration

- **Strict mode** enabled
- **ES2022** target and lib
- **Node.js** module resolution
- **Composite** builds for monorepo optimization

### Nx Configuration

- **Intelligent caching** for faster builds
- **Task dependencies** automatically managed
- **Plugin-based** architecture for extensibility

## 🚀 Creating New Projects

### Generate a new application

```bash
# Create a new Express.js API
npx nx g @nx/express:app my-api

# Create a new React application
npx nx g @nx/web:app my-web-app

# Create a new Node.js application
npx nx g @nx/node:app my-node-app
```

### Generate a new library

```bash
# Create a shared library
npx nx g @nx/js:lib shared-utils

# Create a React component library
npx nx g @nx/react:lib ui-components
```

## 🧪 Testing

### Run tests

```bash
# Test all projects
npx nx run-many --target=test

# Test a specific project
npx nx test my-app

# Test with coverage
npx nx test my-app --coverage
```

## 🏗️ Building

### Build projects

```bash
# Build all projects
npx nx run-many --target=build

# Build a specific project
npx nx build my-app

# Build for production
npx nx build my-app --prod
```

## 🔍 Development

### Start development servers

```bash
# Serve a web application
npx nx serve my-web-app

# Serve an Express API
npx nx serve my-api
```

### Watch for changes

```bash
# Watch all projects
npx nx run-many --target=build --watch

# Watch a specific project
npx nx build my-app --watch
```

## 📊 Project Graph

Visualize your project dependencies:

```bash
npx nx graph
```

This opens an interactive visualization of your monorepo's project dependencies and task relationships.

## 🎨 Code Quality

### Linting and Formatting

```bash
# Check code quality
pnpm check

# Fix issues automatically
pnpm fix
```

### Type Checking

```bash
# Type check all projects
npx nx run-many --target=typecheck

# Type check a specific project
npx nx typecheck my-app
```

## 🔧 Customization

### Adding New Tools

1. Install the desired Nx plugin: `pnpm add -D @nx/plugin-name`
2. Add the plugin to `nx.json` plugins array
3. Generate new projects or targets as needed

### Modifying Biome.js Rules

Edit `biome.jsonc` to customize:

- Linting rules and severity levels
- Formatting preferences
- File inclusion/exclusion patterns

### Extending TypeScript Configuration

- Modify `tsconfig.base.json` for workspace-wide settings
- Create project-specific `tsconfig.json` files for custom configurations

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Run `pnpm check` to ensure code quality
5. Submit a pull request

## 📄 License

This project is licensed under the terms specified in the LICENSE file.

## 🆘 Support

For issues and questions:

- Check the [Nx documentation](https://nx.dev/)
- Review [Biome.js documentation](https://biomejs.dev/)
- Open an issue in this repository

---

**Built with ❤️ by AI Alchemy Labs**
