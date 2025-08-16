# Bodhi Learn Project Structure

This document outlines the folder and file structure of the **Bodhi Learn** platform repository, designed to help developers quickly navigate and understand the codebase organization.

## 📁 Root Directory

```
.
├── .github/           # GitHub Actions and workflows
├── apps/              # Frontend and mobile applications
├── services/          # Backend microservices
├── packages/          # Shared libraries and utilities
├── config/            # Global configurations
├── infra/             # Infrastructure as code
├── scripts/           # Build and utility scripts
├── docs/              # Project documentation
├── tests/             # Test suites
│   ├── unit/          # Unit tests
│   └── integration/   # Integration tests
├── e2e/              # End-to-end tests
├── docker-compose.yml # Local development setup
├── package.json      # Root package configuration
└── README.md         # Project overview
```

## 🖥️ Apps

### Web Application (`/apps/web`)
```
web/
├── public/      # Static assets
├── styles/      # Global styles
├── pages/       # Next.js pages
├── components/  # Reusable components
├── package.json
└── next.config.js
```

### Admin Panel (`/apps/admin`)
```
admin/
├── public/      # Static assets
├── src/         # Source code
├── styles/      # Admin-specific styles
└── package.json
```

### Mobile App (`/apps/mobile`)
```
mobile/
├── assets/      # Images, fonts, etc.
└── package.json
```

## ⚙️ Services

### API Gateway (`/services/api-gateway`)
```
api-gateway/
├── controllers/  # Request handlers
├── models/       # Data models
├── routes/       # API endpoints
└── package.json
```

### Authentication Service (`/services/auth`)
```
auth/
├── controllers/  # Auth logic
├── models/       # User models
├── routes/       # Auth endpoints
├── utils/        # JWT, helpers
└── package.json
```

### Other Services
- `tenant/` - Multi-tenancy management
- `institution/` - Institution management
- `attendance/` - Attendance tracking
- `billing/` - Payment processing

## 📦 Packages

### UI Components (`/packages/ui`)
```
ui/
└── components/  # Shared components
    ├── Button.js
    ├── Card.js
    └── Modal.js
```

### Shared Utilities (`/packages/commons`)
```
commons/
├── logger.js       # Logging utilities
└── errorHandler.js # Error handling
```

### Configuration (`/packages/config`)
```
config/
├── jest.config.js  # Test configuration
├── .eslintrc.js   # Linting rules
└── .prettierrc    # Code formatting
```

## 🚀 Infrastructure

### Docker (`/infra/docker`)
```
docker/
├── Dockerfile         # Container definitions
└── docker-compose.yml # Service orchestration
```

### Kubernetes (`/infra/k8s`)
```
k8s/
└── deployment.yaml  # K8s deployment configs
```

### CI/CD (`/infra/ci-cd`)
```
ci-cd/
└── ci-pipeline.yml  # Pipeline definitions
```

## 📚 Documentation

### Project Docs (`/docs`)
```
docs/
├── architecture.md   # System design
├── roadmap.md        # Development roadmap
├── api-spec.md       # API documentation
└── getting-started.md
```

## 🧪 Testing

### Test Structure
```
tests/
├── unit/                 # Unit tests
│   └── sample.test.js
├── integration/          # Integration tests
│   └── sample.integration.test.js
└── e2e/                  # End-to-end tests
    └── sample.e2e.test.js
```

## 🛠️ Development

### Environment Setup
1. Copy `.env.example` to `.env` and configure
2. Install dependencies: `npm install`
3. Start development server: `npm run dev`

### Scripts
- `npm run test` - Run all tests
- `npm run build` - Build for production
- `npm run lint` - Run linter

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

*Last updated: August 2023*

