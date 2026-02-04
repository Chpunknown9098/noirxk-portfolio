# 🚀 NoirXK Portfolio - AI & Automation Systems Lab

> Portfolio project showcasing system design, automation, and AI integration

[![CI/CD Pipeline](https://github.com/Chpunknown9098/noirxk-portfolio/actions/workflows/ci.yml/badge.svg)](https://github.com/Chpunknown9098/noirxk-portfolio/actions/workflows/ci.yml)

## 📋 Overview

This is a comprehensive portfolio showcasing three key demonstration systems:

1. **AI Assistant for Operations** - Intelligent automation for operational tasks
2. **Revenue Automation System** - Automated revenue tracking and optimization
3. **Operations Dashboard** - Real-time monitoring and analytics

## 🏗️ Architecture

This project uses a **monorepo structure** powered by Turborepo, allowing efficient code sharing and build optimization across multiple applications and packages.

```
noirxk-portfolio/
├── apps/                    # Applications
│   ├── web/                 # Main Next.js application
│   ├── ai-assistant-demo/   # Demo 1: AI Assistant
│   ├── revenue-demo/        # Demo 2: Revenue Automation
│   └── operations-demo/     # Demo 3: Operations Dashboard
├── packages/                # Shared packages
│   ├── ui/                  # Shared UI components
│   ├── config/              # Configuration (ESLint, TypeScript)
│   ├── types/               # Shared TypeScript types
│   ├── simulation/          # API simulation layer
│   └── utils/               # Shared utilities
├── docs/                    # Documentation
└── .github/                 # GitHub Actions & workflows
```

## 🛠️ Tech Stack

- **Framework**: Next.js 14+ (React)
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **Monorepo**: Turborepo
- **Package Manager**: pnpm
- **CI/CD**: GitHub Actions
- **Deployment**: Vercel (or Azure with GitHub Student Pack)

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- pnpm 8+

### Installation

```bash
# Clone the repository
git clone https://github.com/Chpunknown9098/noirxk-portfolio.git
cd noirxk-portfolio

# Install dependencies
pnpm install

# Start development servers for all apps
pnpm dev
```

### Development Commands

```bash
pnpm dev          # Start all apps in development mode
pnpm build        # Build all apps and packages
pnpm lint         # Run ESLint across all packages
pnpm test         # Run tests across all packages
pnpm format       # Format code with Prettier
pnpm clean        # Clean all build artifacts
```

## 📦 Workspaces

### Apps

- **web** - Main portfolio website and navigation
- **ai-assistant-demo** - AI-powered operational assistant demonstration
- **revenue-demo** - Revenue tracking and automation system
- **operations-demo** - Operations monitoring dashboard

### Packages

- **ui** - Shared React components and design system
- **config** - Shared ESLint and TypeScript configurations
- **types** - Shared TypeScript type definitions
- **simulation** - Mock API layer for demonstrations
- **utils** - Common utility functions

## 🎓 GitHub Student Pack Integration

This project is designed to leverage benefits from the GitHub Student Pack:

- ✅ **GitHub Actions** - Free CI/CD (unlimited minutes for public repos)
- 🔄 **GitHub Codespaces** - 60 hours/month free cloud development
- ☁️ **Azure Credits** - $100/year for hosting and services
- 🗄️ **MongoDB Atlas** - Free tier for database
- 🔒 **Namecheap** - Free domain and SSL certificate
- 📊 **Sentry** - Error tracking (500k events/month)

### Future Integrations

- [ ] Deploy to Azure App Service
- [ ] Set up MongoDB Atlas for data persistence
- [ ] Configure custom domain with Namecheap SSL
- [ ] Add error monitoring with Sentry
- [ ] GitHub Copilot integration for AI assistance

## 🧪 Testing

Tests are organized per package/app. Run all tests with:

```bash
pnpm test
```

## 📝 Documentation

Detailed documentation for each component is available in the `/docs` directory.

## 🤝 Contributing

This is a personal portfolio project, but feedback and suggestions are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Kevin V.**

- GitHub: [@Chpunknown9098](https://github.com/Chpunknown9098)

## 🙏 Acknowledgments

- GitHub Education for the Student Developer Pack
- The open-source community

---

**Built with ❤️ using modern web technologies**
