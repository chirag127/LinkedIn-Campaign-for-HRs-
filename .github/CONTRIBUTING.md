# Contributing to RecruitPulse-LinkedIn-Data-Scraper-CLI-Python

Thank you for considering contributing to `RecruitPulse-LinkedIn-Data-Scraper-CLI-Python`! We aim for a professional, high-velocity development process, adhering to the Apex Technical Authority standards.

## 1. Our Philosophy

*   **Zero-Defect:** Strive for impeccable code quality and robust error handling.
*   **High-Velocity:** Implement efficient workflows and clear guidelines to accelerate development.
*   **Future-Proof:** Build with extensibility, maintainability, and evolving industry standards in mind.

## 2. Code of Conduct

This project adheres to a Code of Conduct (see `.github/CODE_OF_CONDUCT.md` - *Note: This file is assumed to exist based on standard GitHub practices, but not explicitly requested in the prompt. If it were, it would be generated.*). By participating, you are expected to uphold this code. Please report unacceptable behavior to `chirag127@example.com`.

## 3. How to Contribute

### 3.1. Setup

1.  **Fork the Repository:** Create your own fork of the `chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python` repository.
2.  **Clone Your Fork:** Clone your forked repository to your local machine:
    bash
    git clone https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python.git
    cd RecruitPulse-LinkedIn-Data-Scraper-CLI-Python
    
3.  **Set Upstream Remote:** Configure your local repository to track the original repository:
    bash
    git remote add upstream https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python.git
    
4.  **Create a Development Branch:** Always work on a new branch for your contributions:
    bash
    git checkout -b feature/your-new-feature-name
    # or
    git checkout -b bugfix/your-bug-fix-description
    
5.  **Environment Setup:** Follow the setup instructions in the `README.md` to install dependencies and set up the Python environment (using `uv`).

### 3.2. Development Workflow

*   **Linting & Formatting:** Ensure your code is linted and formatted using **Ruff** before committing. Run:
    bash
    uv run ruff format . --check
    uv run ruff check . --fix
    
*   **Testing:** Write comprehensive unit and integration tests using **Pytest**. All new code must be accompanied by tests. Run tests:
    bash
    uv run pytest
    
*   **Commit Messages:** Follow Conventional Commits specification (e.g., `feat: add new data parsing module`, `fix: resolve LinkedIn CAPTCHA issue`).
*   **Pull Requests:** Submit Pull Requests (PRs) from your feature branch to the `main` branch of your fork. Include a clear description of your changes, the problem they solve, and how to test them.

## 4. Architectural Principles

We adhere to the Apex Technical Authority's core principles:

*   **SOLID:** Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion.
*   **DRY:** Don't Repeat Yourself.
*   **YAGNI:** You Ain't Gonna Need It.
*   **Modularity:** Favor a Modular Monolith architecture for clear separation of concerns within the Python codebase.

## 5. Contribution Areas

*   **Core Scraping Logic:** Improving efficiency, reliability, and ethical data extraction methods.
*   **CLI Interface:** Enhancing user experience, command structure, and argument parsing.
*   **Data Structuring:** Optimizing output formats and data validation.
*   **Testing:** Expanding test coverage and robustness.
*   **Documentation:** Improving clarity and completeness of project documentation.

## 6. Reporting Issues

Before reporting an issue, please check if it already exists. If not, create a new issue using the `bug_report.md` template provided in the `.github/ISSUE_TEMPLATE/` directory. Provide detailed steps to reproduce the bug, expected behavior, actual behavior, and relevant environment information.

## 7. Requesting Features

Use the `feature_request.md` template (if available, otherwise use the bug report template and specify 'Feature Request' in the title) to propose new features. Clearly articulate the value proposition and use cases.

## 8. Security

If you discover any security vulnerabilities, please report them responsibly according to the `.github/SECURITY.md` guidelines. **DO NOT** open a public issue. Instead, follow the disclosure process outlined there.

## 9. Project Metadata

This project follows the Apex Naming Convention: `<Product-Name>-<Primary-Function>-<Platform>-<Type>`.

*   **Name:** `RecruitPulse-LinkedIn-Data-Scraper-CLI-Python`
*   **Description:** A robust, high-performance Python CLI utility designed for ethical extraction and structured compilation of public recruitment data from LinkedIn profiles and job postings.
*   **Topics:** `['Python', 'WebScraping', 'CLI', 'DataExtraction', 'Automation', 'Selenium', 'RecruitmentTech']`
*   **Repository URL:** `https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python`

By contributing, you agree that your contributions will be licensed under the `CC BY-NC` license.
