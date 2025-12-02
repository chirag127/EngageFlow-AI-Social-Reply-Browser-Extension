# Contributing to EngageFlow

First, thank you for considering contributing to EngageFlow. It's people like you that make this project a world-class tool. We hold our codebase to the highest professional standards to ensure reliability, maintainability, and performance.

This document provides guidelines for contributing. Please read it carefully to ensure a smooth and effective workflow.

## 📜 Core Principles & Code of Conduct

We operate on a set of core principles that define our engineering culture. For a detailed overview of our architectural standards, tech stack, and AI agent directives, please review the [**AGENTS.md**](./AGENTS.md) file.

All contributors are expected to adhere to our [Code of Conduct](./CODE_OF_CONDUCT.md) to foster an open, inclusive, and professional environment.

## 🚀 Getting Started: Your First Contribution

Contributions can range from fixing a typo in the documentation to implementing a major new feature. Unsure where to start? Look for issues tagged `good first issue` or `help wanted`.

🔗 **[Browse Open Issues](https://github.com/chirag127/EngageFlow-AI-Social-Reply-Browser-Extension/issues)**

### Prerequisites

Ensure you have the following installed on your local development machine:

-   **Node.js**: `v20.x` or later (LTS recommended)
-   **pnpm**: A fast, disk space-efficient package manager. Install via `npm install -g pnpm`.
-   **Git**: For version control.

### Development Environment Setup

1.  **Fork the Repository**
    Click the "Fork" button at the top-right of the [repository page](https://github.com/chirag127/EngageFlow-AI-Social-Reply-Browser-Extension) to create a copy under your own GitHub account.

2.  **Clone Your Fork**
    Clone your forked repository to your local machine:
    bash
    git clone https://github.com/YOUR_USERNAME/EngageFlow-AI-Social-Reply-Browser-Extension.git
    cd EngageFlow-AI-Social-Reply-Browser-Extension
    

3.  **Install Dependencies**
    Install the project dependencies using `pnpm`:
    bash
    pnpm install
    

4.  **Run the Development Server**
    This command will build the extension and watch for file changes, rebuilding automatically:
    bash
    pnpm dev
    

5.  **Load the Extension in Your Browser**
    -   Open Chrome and navigate to `chrome://extensions`.
    -   Enable "Developer mode" (top-right toggle).
    -   Click "Load unpacked".
    -   Select the `dist` directory generated in the project root.

## 🛠️ Development Workflow

### Branching Strategy

Create a new branch for every feature or fix. Use the following naming convention:

-   **Features**: `feature/short-description` (e.g., `feature/add-linkedin-support`)
-   **Fixes**: `fix/issue-description` (e.g., `fix/reply-button-alignment`)
-   **Documentation**: `docs/update-readme`
-   **Refactoring**: `refactor/simplify-api-service`

bash
git checkout -b feature/your-new-feature


### Code Quality and Standards

We use **Biome** for linting and formatting to maintain consistent code style. Before committing, run the following commands:

bash
# Check for linting errors
pnpm lint

# Automatically format all files
pnpm format


### Testing

High-quality testing is mandatory. All new features must be accompanied by relevant unit or integration tests.

bash
# Run all unit and integration tests
pnpm test


### Commit Message Convention

We enforce the [**Conventional Commits**](https://www.conventionalcommits.org/en/v1.0.0/) specification. This helps automate changelogs and provides a clear, structured commit history.

**Format**: `<type>(<scope>): <subject>`

-   **`feat`**: A new feature.
-   **`fix`**: A bug fix.
-   **`docs`**: Documentation only changes.
-   **`style`**: Changes that do not affect the meaning of the code (white-space, formatting, etc).
-   **`refactor`**: A code change that neither fixes a bug nor adds a feature.
-   **`perf`**: A code change that improves performance.
-   **`test`**: Adding missing tests or correcting existing tests.
-   **`build`**: Changes that affect the build system or external dependencies.
-   **`ci`**: Changes to our CI configuration files and scripts.

**Example:**
`feat(ui): implement settings modal for tone adjustment`

## 📦 Submitting Your Pull Request

1.  **Push Your Changes**
    Push your feature branch to your forked repository:
    bash
    git push origin feature/your-new-feature
    

2.  **Create a Pull Request (PR)**
    -   Navigate to the [original repository](https://github.com/chirag127/EngageFlow-AI-Social-Reply-Browser-Extension) and you will see a prompt to create a PR from your recently pushed branch.
    -   Set the target branch to `main`.
    -   Fill out the [**Pull Request Template**](./PULL_REQUEST_TEMPLATE.md) completely. Provide a clear title and a detailed description of your changes. Link any relevant issues (e.g., `Closes #123`).

3.  **Code Review**
    -   A core maintainer will review your PR.
    -   Ensure all automated CI checks pass successfully.
    -   Address any feedback or requested changes promptly.
    -   Once approved, your PR will be squashed and merged into the `main` branch.

Thank you for contributing to the future of intelligent social engagement!