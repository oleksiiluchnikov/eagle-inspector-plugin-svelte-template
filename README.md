# Eagle Plugin Svelte Template

This is a template repository for creating plugins for [Eagle](https://en.eagle.cool/) using Svelte and Vite. It provides a solid foundation for building powerful and efficient Eagle plugins with modern web technologies.

## Features

- 🚀 Built with [Svelte](https://svelte.dev/) and [Vite](https://vitejs.dev/)
- 📦 Optimized build configuration for Eagle plugins
- 🔧 Ready-to-use development environment with hot reload
- 📝 Well-documented template structure
- 🎨 Theme-aware components that match Eagle's UI
- 🛠️ TypeScript support out of the box
- 📚 Comprehensive component library
- 🧪 Testing setup with Jest
- 🔍 ESLint and Prettier for code quality</REPLACE>

## Getting Started

### Prerequisites

- Node.js 18+
- Eagle Application installed
- Basic knowledge of Svelte and JavaScript/TypeScript

### Use this template

1. Click the "Use this template" button on GitHub
2. Clone your new repository
3. Install dependencies:

```bash
npm install
```

### Development

Start the development server:

```bash
npm run dev
```

This will:

- Start Vite dev server with hot module reloading
- Watch for file changes and automatically rebuild
- Provide hot reloading in Eagle when files change

### Building

Build your plugin for production:

```bash
npm run build
```

The built files will be in the `build` directory.

### Testing in Eagle

1. Launch Eagle application
2. Go to Plugins -> Developer Options
3. Click "Import Local Project"
4. Select your plugin directory
5. The plugin will appear in Eagle's plugin list

### TypeScript Support

This template includes TypeScript support out of the box. To use TypeScript:

1. Rename your .js/.svelte files to .ts/.svelte
2. Add types to your variables and functions
3. Use the built-in Eagle type definitions

Example:

```typescript
interface EagleImage {
  id: string;
  name: string;
  url: string;
  // ... other properties
}

function processImage(image: EagleImage): void {
  // Your code here
}
```

## Project Structure

```
/
├── src/
│   ├── components/    # Reusable UI components
│   │   ├── Button.svelte
│   │   ├── Input.svelte
│   │   └── ...
│   ├── lib/          # Utility functions and helpers
│   │   ├── api.ts    # Eagle API wrapper
│   │   └── theme.ts  # Theme utilities
│   ├── types/        # TypeScript type definitions
│   │   └── eagle.d.ts
│   ├── main.ts       # Entry point
│   └── App.svelte    # Root component
├── public/           # Static assets
│   ├── logo.png
│   └── ...
├── tests/           # Test files
├── docs/            # Documentation
├── .github/         # GitHub workflows
├── vite.config.ts   # Vite configuration
├── tsconfig.json    # TypeScript configuration
├── manifest.json    # Eagle plugin manifest
└── package.json     # Project configuration
```

## Available Components

This template includes several pre-built components that match Eagle's UI:

- `Button.svelte` - Standard button component with proper theming

## License

[MIT](https://choosealicense.com/licenses/mit/)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
