<div align="center">
  <h1>🚀 Next.js Web Boilerplate</h1>
  <p><strong>A comprehensive, production-ready Next.js boilerplate with enterprise-grade features</strong></p>
  <p><em>Built for scalability, performance, and developer productivity</em></p>
  <p>
    <img src="https://img.shields.io/badge/Next.js-14.0-black?style=flat-square&logo=next.js" alt="Next.js">
    <img src="https://img.shields.io/badge/TypeScript-5.3-blue?style=flat-square&logo=typescript" alt="TypeScript">
    <img src="https://img.shields.io/badge/React-18.2-61DAFB?style=flat-square&logo=react" alt="React">
    <img src="https://img.shields.io/badge/MUI-5.14-007FFF?style=flat-square&logo=mui" alt="MUI">
    <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="License">
  </p>
</div>

## ✨ Features

- **⚡ Next.js 14** - Latest Next.js with App Router and Server Components
- **📘 TypeScript** - Full type safety with strict configuration
- **🎨 Material-UI 5** - Modern React component library
- **🔄 TanStack Query** - Powerful data fetching and caching
- **📈 State Management** - Zustand for global state management
- **🌍 Internationalization** - Multi-language support with next-international
- **🔥 Firebase Integration** - Push notifications and analytics
- **📏 Performance Monitoring** - New Relic integration
- **🛡️ Security Headers** - Advanced security configuration
- **🧪 Testing Suite** - Jest and React Testing Library
- **🗺️ Bundle Analysis** - Built-in bundle analyzer
- **🐳 Docker Ready** - Containerization support
- **📄 Code Generation** - CLI scripts for components, domains, and features
- **📋 Code Quality** - ESLint, Prettier, Husky, and Commitizen
- **🏗️ Clean Architecture** - Domain-driven design structure

## 🏗️ Architecture

This boilerplate follows **Clean Architecture** principles with a feature-based folder structure:

- **Domain Layer**: Business logic and entities
- **Application Layer**: Use cases and application services
- **Infrastructure Layer**: External services and repositories
- **Presentation Layer**: React components and pages

## 🏗️ Tech Stack

### **Frontend Framework**
- **[Next.js 14.0](https://nextjs.org)** - React framework with SSR/SSG
- **[React 18.2](https://react.dev)** - UI library with concurrent features
- **[TypeScript 5.3](https://www.typescriptlang.org)** - Static type checking

### **UI & Styling**
- **[Material-UI 5.14](https://mui.com)** - React component library
- **[Emotion 11](https://emotion.sh)** - CSS-in-JS library
- **[Material Icons](https://mui.com/material-ui/material-icons/)** - Google Material Icons

### **State Management & Data Fetching**
- **[Zustand 4.4](https://zustand-demo.pmnd.rs)** - Lightweight state management
- **[TanStack Query 5.8](https://tanstack.com/query)** - Data fetching and caching
- **[Axios 1.6](https://axios-http.com)** - HTTP client
- **[Zod 3.22](https://zod.dev)** - Schema validation

### **Internationalization & Utilities**
- **[Next International 1.1](https://github.com/QuiiBz/next-international)** - i18n solution
- **[date-fns 2.30](https://date-fns.org)** - Date utility library
- **[Sharp 0.32](https://sharp.pixelplumbing.com)** - Image optimization

### **Development & Build Tools**
- **[Turbopack](https://turbo.build/pack)** - Fast development server (optional)
- **[Bundle Analyzer](https://www.npmjs.com/package/@next/bundle-analyzer)** - Bundle size analysis
- **[SVGR](https://react-svgr.com)** - SVG to React components

### **Testing & Quality**
- **[Jest 29.7](https://jestjs.io)** - JavaScript testing framework
- **[React Testing Library 14.1](https://testing-library.com)** - React component testing
- **[ESLint 8.54](https://eslint.org)** - Code linting
- **[Prettier 3.1](https://prettier.io)** - Code formatting
- **[Husky 8.0](https://typicode.github.io/husky/)** - Git hooks
- **[Commitizen](http://commitizen.github.io/cz-cli/)** - Conventional commits

### **Monitoring & Analytics**
- **[New Relic](https://newrelic.com)** - Application performance monitoring
- **[Firebase 10.6](https://firebase.google.com)** - Push notifications and analytics

## 📋 Prerequisites

- **Node.js** 18.0 or later (see `.nvmrc` for exact version)
- **npm**, **yarn**, **pnpm**, or **bun** package manager
- **Git** for version control
- **Docker** (optional, for containerization)

## 🚀 Quick Start

### 1. Clone Repository

```bash
git clone <repository-url>
cd next-web-boilerplate
```

### 2. Install Dependencies

```bash
npm install
# or
yarn install
# or
pnpm install
# or
bun install
```

### 3. Environment Setup

```bash
# Copy environment variables
cp .env.example .env.local
```

Configure your environment variables:

```env
# Application
APP_ENV=development
NEXT_PUBLIC_BASE_URL=http://localhost:3000
NEXT_PUBLIC_API_URL=

# Firebase (optional)
NEXT_PUBLIC_FIREBASE_API_KEY=your-api-key
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your-project-id
# ... other Firebase config

# New Relic (optional)
NEW_RELIC_LICENSE_KEY=your-license-key
```

### 4. Start Development Server

```bash
# Standard development server
npm run dev

# With Turbopack (faster)
npm run dev:turbo
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## 📜 Available Scripts

| Script | Description | Usage |
|--------|-------------|-------|
| `dev` | Start development server with New Relic | `npm run dev` |
| `dev:turbo` | Start development server with Turbopack | `npm run dev:turbo` |
| `build` | Build for production | `npm run build` |
| `build:analyze` | Build with bundle analysis | `npm run build:analyze` |
| `start` | Start production server | `npm start` |
| `lint` | Run ESLint | `npm run lint` |
| `prettier` | Format code with Prettier | `npm run prettier` |
| `test` | Run tests in watch mode | `npm test` |
| `test:coverage` | Run tests with coverage | `npm run test:coverage` |
| `test:dev` | Run tests in development mode | `npm run test:dev` |
| `test:clear` | Clear Jest cache | `npm run test:clear` |

### **Code Generation Scripts**

| Script | Description | Usage |
|--------|-------------|-------|
| `generate:component` | Generate new component | `npm run generate:component` |
| `generate:domain` | Generate new domain entity | `npm run generate:domain` |
| `generate:feature` | Generate new feature module | `npm run generate:feature` |
| `generate:service` | Generate new service | `npm run generate:service` |
| `generate:store` | Generate new Zustand store | `npm run generate:store` |
| `generate:useCase` | Generate new use case | `npm run generate:useCase` |

## 🗺️ Project Structure

```
next-web-boilerplate/
├── src/
│   ├── components/          # Reusable UI components
│   │   └── Header/          # Example header component
│   ├── constants/           # Application constants
│   │   ├── configs.ts       # App configuration
│   │   ├── featureFlags.ts  # Feature flags
│   │   ├── images.ts        # Image constants
│   │   ├── routes.ts        # Route definitions
│   │   └── storageKey.ts    # Storage keys
│   ├── domains/            # Domain entities (Business Logic)
│   │   ├── Auth.ts          # Authentication domain
│   │   ├── Example.ts       # Example domain
│   │   ├── Response.ts      # API response domain
│   │   ├── __mocks__/       # Domain mocks for testing
│   │   └── __tests__/       # Domain unit tests
│   ├── features/           # Feature modules
│   │   └── Example/         # Example feature
│   │       ├── index.tsx    # Feature component
│   │       ├── configs.ts   # Feature config
│   │       ├── styles.ts    # Feature styles
│   │       └── types.ts     # Feature types
│   ├── helpers/            # Utility functions
│   │   ├── cache.ts         # Cache utilities
│   │   ├── error.ts         # Error handling
│   │   └── __tests__/       # Helper unit tests
│   ├── hooks/              # Custom React hooks
│   ├── pages/              # Next.js pages
│   ├── services/           # External service integrations
│   ├── stores/             # Zustand stores
│   ├── styles/             # Global styles
│   ├── types/              # TypeScript type definitions
│   └── __mocks__/          # Global mocks for testing
├── scripts/               # Code generation scripts
│   ├── create-component.js # Component generator
│   ├── create-domain.js    # Domain generator
│   ├── create-feature.js   # Feature generator
│   ├── create-service.js   # Service generator
│   ├── create-store.js     # Store generator
│   └── create-use-case.js  # Use case generator
├── public/               # Static assets
├── .env.example          # Environment variables template
├── .nvmrc               # Node.js version specification
├── Dockerfile           # Docker configuration
├── jest.config.js       # Jest testing configuration
├── next.config.js       # Next.js configuration
└── tsconfig.json        # TypeScript configuration
```

## 🌍 Internationalization

The boilerplate includes built-in i18n support:

- **Supported Languages**: Indonesian (`id`), English (`en`)
- **Default Language**: Indonesian
- **Configuration**: `next.config.js`
- **Library**: `next-international`

```javascript
// next.config.js
i18n: {
  locales: ['id', 'en'],
  defaultLocale: 'id',
  localeDetection: false,
}
```

## 🛡️ Security Features

Advanced security headers are automatically applied:

- **HSTS** - HTTP Strict Transport Security
- **X-Frame-Options** - Clickjacking protection
- **X-XSS-Protection** - XSS filtering
- **X-Content-Type-Options** - MIME type sniffing protection
- **Referrer-Policy** - Referrer information control
- **DNS Prefetch Control** - DNS prefetching control

## 🧪 Testing

### **Unit Testing**
```bash
# Run all tests
npm test

# Run tests with coverage
npm run test:coverage

# Run tests in development mode with coverage
npm run test:dev
```

### **Test Configuration**
- **Framework**: Jest with React Testing Library
- **Environment**: jsdom for React component testing
- **Coverage**: Istanbul coverage reports
- **Mocks**: Comprehensive mocking for external dependencies

### **Testing Structure**
- Domain tests: `src/domains/__tests__/`
- Helper tests: `src/helpers/__tests__/`
- Component tests: Co-located with components
- Mocks: `src/__mocks__/` and `src/domains/__mocks__/`

## 📈 Performance Monitoring

### **New Relic Integration**
The boilerplate includes New Relic for application performance monitoring:

- **Server-side monitoring** - API performance and errors
- **Browser monitoring** - Frontend performance metrics
- **Custom metrics** - Business-specific tracking

### **Bundle Analysis**
```bash
# Analyze bundle size
npm run build:analyze
```

### **Performance Features**
- **Image optimization** with Sharp
- **Font optimization** with next/font
- **Automatic code splitting**
- **Static site generation** support
- **Advanced caching** strategies

## 🔥 Firebase Integration

### **Push Notifications**
```javascript
// Environment variables for Firebase
NEXT_PUBLIC_FIREBASE_API_KEY=
NEXT_PUBLIC_FIREBASE_PROJECT_ID=
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=
NEXT_PUBLIC_FIREBASE_APP_ID=
NEXT_PUBLIC_FIREBASE_VAPID_KEY=
```

### **Features**
- **Cloud Messaging** - Push notifications
- **Analytics** - User behavior tracking
- **Performance Monitoring** - Real user metrics

## 🐳 Docker Support

### **Build Docker Image**
```bash
# Build image
docker build -t next-web-boilerplate .

# Run container
docker run -p 3000:3000 next-web-boilerplate
```

### **Docker Features**
- **Multi-stage build** - Optimized image size
- **Production ready** - Minimal runtime dependencies
- **Security** - Non-root user execution

## 🛠️ Code Generation

Use the built-in generators to scaffold new code:

### **Generate Component**
```bash
npm run generate:component
# Creates: src/components/[Name]/index.tsx + types.ts
```

### **Generate Feature**
```bash
npm run generate:feature
# Creates: src/features/[Name]/ with complete structure
```

### **Generate Domain**
```bash
npm run generate:domain
# Creates: src/domains/[Name].ts with tests and mocks
```

### **Generate Store**
```bash
npm run generate:store
# Creates: src/stores/[name]Store.ts with Zustand setup
```

## 🚀 Deployment

### **Vercel (Recommended)**
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel --prod
```

### **Environment Variables for Production**
```env
APP_ENV=production
NEXT_PUBLIC_BASE_URL=https://your-domain.com
NEXT_PUBLIC_API_URL=https://api.your-domain.com
NEW_RELIC_LICENSE_KEY=your-production-key
# ... other production configs
```

## 📋 Best Practices

### **Code Organization**
- Follow clean architecture principles
- Keep components focused and reusable
- Use TypeScript interfaces for all data structures
- Implement proper error boundaries

### **Performance**
- Use Next.js Image component for optimizations
- Implement proper caching strategies
- Lazy load components when appropriate
- Monitor bundle size regularly

### **Testing**
- Write unit tests for business logic (domains)
- Test components with React Testing Library
- Mock external dependencies consistently
- Maintain high test coverage

### **Security**
- Keep dependencies updated
- Use environment variables for sensitive data
- Implement proper CORS policies
- Follow OWASP security guidelines

## 🔧 Development Guidelines

### **Git Workflow**
- Use conventional commits (Commitizen)
- Pre-commit hooks ensure code quality
- Branch naming: `feature/`, `bugfix/`, `hotfix/`

### **Code Quality**
- ESLint for code linting
- Prettier for code formatting
- TypeScript strict mode enabled
- Husky for git hooks enforcement

### **Commit Messages**
```bash
# Use Commitizen for conventional commits
npx cz
# or
git cz
```

## 🤝 Contributing

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes using Commitizen (`npm run commit`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### **Development Setup**
```bash
# Clone and setup
git clone <your-fork>
cd next-web-boilerplate
npm install
cp .env.example .env.local

# Start development
npm run dev

# Run tests
npm test

# Check code quality
npm run lint
npm run prettier
```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Next.js Team](https://nextjs.org)
- [Material-UI](https://mui.com)
- [TanStack](https://tanstack.com)
- [Vercel](https://vercel.com)
- [New Relic](https://newrelic.com)
- [Firebase](https://firebase.google.com)
