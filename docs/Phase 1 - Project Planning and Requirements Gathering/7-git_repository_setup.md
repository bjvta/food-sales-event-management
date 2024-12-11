
# Git Repository Setup and CI/CD Pipeline

## Repository Structure

```plaintext
food-sales-event-management-system/
├── docs/                 # Documentation for all project phases
│   ├── phase1/           # Requirements, wireframes, architecture
│   ├── phase2/           # Milestones and sprints
├── rails-backend/        # Rails project folder
├── react-frontend/       # React project folder
├── README.md             # Project overview
└── .gitignore            # Files to ignore
```

---

## Branching Strategy

### Initial Branches
- **`backend`**: For Rails API development.
- **`frontend`**: For React with TypeScript development.
- **`graphql-schema`**: For shared GraphQL schema definitions.

---

## CI/CD Pipeline

### Backend (Rails)
- Tool: **GitHub Actions**
- File: `.github/workflows/backend.yml`
- Workflow:
  1. Checkout the repository.
  2. Set up Ruby environment.
  3. Install dependencies (`bundle install`).
  4. Run tests (`bundle exec rspec`).

### Frontend (React with TypeScript)
- Tool: **GitHub Actions**
- File: `.github/workflows/frontend.yml`
- Workflow:
  1. Checkout the repository.
  2. Set up Node.js environment.
  3. Install dependencies (`npm install`).
  4. Run tests (`npm test`).
  5. Check build integrity (`npm run build`).

---

## Code Review Guidelines

### Pull Request Standards
1. Link PRs to tasks or issues.
2. Include a detailed description of changes.
3. Ensure all CI tests pass before review.

### Code Style
- **Backend**: Follow Ruby style guide (`rubocop`).
- **Frontend**: Use ESLint with TypeScript rules.

### Review Process
- At least one reviewer must approve before merging.

### Branch Protection
- Protect the `main` branch.
- Require passing CI checks before merging.

---

## Deliverables

1. **Git Repository**:
   - A structured repository with branches for `frontend`, `backend`, and `graphql-schema`.

2. **CI/CD Pipeline**:
   - Backend tests with RSpec.
   - Frontend tests with Jest and build integrity checks.

3. **Documentation**:
   - Markdown files summarizing each phase in the `docs/` folder.
