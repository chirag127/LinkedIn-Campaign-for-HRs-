# RecruitPulse: LinkedIn Data Scraper CLI Python

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python/ci.yml?style=flat-square)](https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python/actions)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python?style=flat-square)](https://codecov.io/gh/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python)
[![Tech Stack](https://img.shields.io/badge/Python-3.10%2B-blue?style=flat-square&logo=python)](https://www.python.org/)
[![Lint/Format](https://img.shields.io/badge/Ruff-Fast-F25F5F?style=flat-square&logo=ruff)](https://github.com/charliermarsh/ruff)
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-orange?style=flat-square)](https://creativecommons.org/licenses/by-nc/4.0/)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python?style=flat-square)](https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python/stargazers)

[⭐ Star this Repo](https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python)

A high-performance Python CLI utility designed for ethical extraction and structured compilation of public recruitment data from LinkedIn profiles and job postings.

---

## Table of Contents

*   [Features](#features)
*   [Architecture](#architecture)
*   [AI Agent Directives](#ai-agent-directives)
*   [Development Setup](#development-setup)
*   [Usage](#usage)
*   [Testing](#testing)
*   [Contributing](#contributing)
*   [License](#license)

---

## Features

*   **Ethical Data Extraction:** Focuses solely on publicly available recruitment information.
*   **Structured Output:** Compiles data into easily digestible formats (e.g., CSV, JSON).
*   **LinkedIn Focus:** Tailored for LinkedIn job postings and professional profiles.
*   **CLI Interface:** User-friendly command-line interactions.
*   **Automation Ready:** Designed for integration into larger recruitment workflows.

---

## Architecture

This project follows a **Modular Monolith** architecture, ensuring a clear separation of concerns while maintaining a unified codebase for efficient development and deployment. Key components include:

ascii
RecruitPulse/
├── src/
│   ├── cli/
│   │   └── __init__.py  # CLI entry points
│   ├── data/
│   │   ├── extraction/  # Web scraping logic (Selenium, etc.)
│   │   └── processing/  # Data structuring and formatting
│   ├── utils/
│   │   └── __init__.py  # Helper functions
│   └── __init__.py
├── tests/
│   ├── unit/
│   └── integration/
├── pyproject.toml
├── README.md
└── AGENTS.md


---

## 🤖 AI Agent Directives

<details>
<summary>View AI Agent Directives</summary>

### Core Directives

*   **Identity:** Senior Principal Software Architect, Master Technical Copywriter, 40+ years elite experience.
*   **Philosophy:** Zero-Defect, High-Velocity, Future-Proof.
*   **Output Standard:** Execution-only.

### Input Processing & Cognition

*   **Speech-to-Text Interpretation:** Strictly forbid execution of literal typos. Infer technical intent based on project context. Treat `README.md` as SSOT.
*   **Mandatory MCP Instrumentation:** No guessing. Research industry standards, security threats, and UI trends (December 2025 context). Validate external APIs.

### Context-Aware Apex Tech Stacks (Late 2025 Standards)

*   **Python Stack:** Python 3.10+, **uv** (package management), **Ruff** (linting/formatting), **Pytest** (testing).
*   **Architecture:** Modular Monolith.
*   **CLI Framework:** **Click** (or similar) for CLI.
*   **Web Scraping:** Primarily **Selenium** (with appropriate ethical considerations and rate limiting).

### Testing Protocols

*   **Unit Tests:** Comprehensive unit tests for all modules using `pytest`.
*   **Integration Tests:** Tests to ensure seamless interaction between components, especially CLI and data extraction/processing.
*   **E2E Tests:** Simulate real user interactions via CLI commands.

### Security & Compliance

*   **Ethical Scraping:** Adhere strictly to LinkedIn's Terms of Service and robots.txt. Implement rate limiting and user-agent rotation.
*   **Data Privacy:** Handle extracted data with utmost care, focusing on public information only.
*   **License:** CC BY-NC 4.0.

### Versioning & Deployment

*   **Versioning:** Semantic Versioning (SemVer).
*   **CI/CD:** GitHub Actions for automated testing, linting, and package building.

</details>

---

## Development Setup

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python.git
    cd RecruitPulse-LinkedIn-Data-Scraper-CLI-Python
    

2.  **Set up the Python environment using `uv`:**
    bash
    uv venv  # Creates a virtual environment
    uv pip install --editable '.[dev]' # Installs dependencies, including development tools
    
    *(Note: Ensure you have Python 3.10+ installed.)*

3.  **Install Playwright browsers (if using Playwright for E2E testing):**
    bash
    playwright install
    

---

## Usage

*   **Run the CLI help:**
    bash
    python -m recruitpulse --help
    

*   **Example command (hypothetical):**
    bash
    python -m recruitpulse scrape --profile linkedin.com/in/exampleuser --output data.csv
    

*(Refer to the CLI help for detailed command structure and options.)*

---

## Testing

*   **Run linters and formatters:**
    bash
    uv pip run -m ruff check . --fix
    uv pip run -m ruff format .
    

*   **Run unit and integration tests:**
    bash
    uv pip run -m pytest
    

---

## Contributing

Contributions are welcome! Please refer to the [CONTRIBUTING.md](https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python/blob/main/.github/CONTRIBUTING.md) file for detailed guidelines.

---

## License

This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0). See the [LICENSE](https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python/blob/main/LICENSE) file for more details.
