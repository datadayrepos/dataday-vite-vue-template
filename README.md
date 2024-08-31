# Vue-Vite component library template

Vue-Vite component Template is a starter template for swiftly building a component library package with a well-defined, easy-to-use structure.

## 🚀 Features
- **TypeScript Configurations**: Pre-configured TypeScript for smooth development.
- **Eslint Setup**: Pre-configured ESLint with established rules for maintaining code quality.
- **Script Shortcuts**: Pre-defined NPM scripts for common tasks like linting, building, and publishing.
- **Version Management**: Simplifies version bumping and publishing with `bumpp` and `pnpm`.
- **Export Control**: Clearly defined export settings for various module types.
- **LIVE view**: View components live while developing.
- **Documentation**: Live documentation and testing sing vitepress.

## 🛠 Usage

## 1. Clone & Install
Clone this template and navigate to the project directory. Use `pnpm` for installing dependencies:

```sh
git clone https://github.com/datadayrepos/vite-vue-library.git my-new-package
cd my-new-package
pnpm install
```

## 2. Configure
Utilize placeholders for easy setup:
Replace all placeholders (__PLACEHOLDER__) in package.json with your package specifics. E.g., __PACKAGE_NAME__, __AUTHOR_NAME__, etc.

Seach and replace for:
__PACKAGE_NAME__ => the package name
__AUTHOR_NAME__ =>
__GITHUB_USERNAME__ =>
__REPOSITORY_NAME__ =>
__BRAND_NAME__ =>

## 3. Documentation and live view
We combine live-view and documentation of the component using VitePress.
Build doc pages and example code files using the patterns shown in the vite press folder.

Update the '.vitepress/config.mts' file for routing. Insert a line into "function getComponents() "

```sh
# Starts vitepress dev server
pnpm dev
```

## 4. Develop
Your src directory is where your TypeScript source files reside. Transpiled files are output to the dist directory.

## 💻 Commands

Build: Transpile TypeScript to JavaScript
```sh
pnpm build
```

Linting: Check and fix code style
```sh
pnpm lint
pnpm lint:fix
```

Release: Bump version and publish
```sh
pnpm release
```

Testing: Run tests (tbd)
```sh
pnpm run test
```

Type Checking: Validate TypeScript
```sh
pnpm typecheck
```

Publish: Publish package publicly
```sh
pnpm pub
```

## 📦 Template Structure
```json
{
  "name": "__PACKAGE_NAME__",
  "type": "module",
  "version": "0.0.1",
  "private": true,
  "description": "__PACKAGE_DESCRIPTION__",
  ...
  "scripts": {
    "lint": "eslint --cache .",
    "lint:fix": "eslint . --fix",
    "release": "bumpp -r && pnpm -r publish",
    "test": "echo \"Error: no test specified\" && exit 1",
    "typecheck": "tsc --noEmit",
    "build": "tsc",
    "pub": "npm publish --access public"
  },
  ...
}

```

## 🗂️ File Structure
- src/: Source files written in TypeScript.
- dist/: Transpiled source files in JavaScript.

## 🔗 Links
- **Repository**: [GitHub Repository](https://github.com/datadayrepos/vite-vue-library)
- **Issues**: [Report Bugs](https://github.com/datadayrepos/vite-vue-library/issues)


## 📄 License
[MIT](./LICENSE) License &copy; [DataDayRepos](https://github.com/datadayrepos)
