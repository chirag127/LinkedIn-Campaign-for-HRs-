# RecruitPulse-LinkedIn-Data-Scraper-CLI-Python

A robust, high-performance Python CLI utility designed for ethical extraction and structured compilation of public recruitment data from LinkedIn profiles and job postings.

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python/ci.yml?label=Build&style=flat-square)](https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python?label=Coverage&style=flat-square)](https://codecov.io/gh/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python)
[![Python Version](https://img.shields.io/badge/python-3.10%2B-blue?style=flat-square)](https://www.python.org/)
[![Linter](https://img.shields.io/badge/lint--formatter-ruff-black?style=flat-square)](https://github.com/astral-sh/ruff)
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-orange?style=flat-square)](https://creativecommons.org/licenses/by-nc/4.0/)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python?style=flat-square)](https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python)

---


## :star: Star this Repo

If you find this project useful, please consider starring it on GitHub to show your support!

---


## Overview

RecruitPulse is an advanced Python Command-Line Interface (CLI) tool engineered for the ethical and structured scraping of public recruitment data from LinkedIn. It automates the tedious process of gathering information from profiles and job postings, organizing it into a usable format for recruiters and talent acquisition specialists.

## Architecture

This project follows a **Modular Monolith** architecture, ensuring clear separation of concerns while maintaining a unified codebase for efficient development and deployment.

mermaid
graph TD
    A[CLI Interface (Click)] --> B(Core Logic)
    B --> C{LinkedIn API/Web Scraping Adapters}
    C --> D[Data Processing & Structuring]
    D --> E[Output Management (CSV, JSON)]
    B --> F[Configuration Management]
    F --> G[Logging]


## Table of Contents

*   [Overview](#overview)
*   [Architecture](#architecture)
*   [Table of Contents](#table-of-contents)
*   [AI Agent Directives](#robot-ai-agent-directives)
*   [Development Standards](#building-the-project)
    *   [Prerequisites](#prerequisites)
    *   [Setup](#setup)
    *   [Scripts](#scripts)
*   [Principles](#development-principles)
*   [Contributing](#contributing)
*   [License](#license)

## :robot: AI Agent Directives

<details>
<summary>View AI Agent Directives</summary>

### 1. Identity & Prime Directive
*   **Role:** Senior Principal Software Architect, Master Technical Copywriter.
*   **Experience:** 40+ years of elite industry expertise.
*   **Standard:** FAANG-level, "Managing the Unmanageable."
*   **Date Context:** December 2025 (Building for 2026).
*   **Output:** EXECUTION-ONLY. No plans, only executed code, updated docs, applied fixes.
*   **Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. Input Processing & Cognition
*   **Speech-to-Text:** Infer technical intent; **STRICTLY FORBIDDEN** from executing literal typos.
*   **Logic Anchor:** `README.md` is the Single Source of Truth (SSOT).
*   **MCP Instrumentation:**
    *   No Guessing.
    *   Use `linkup`/`brave` for December 2025 industry standards, security threats, and 2026 trends.
    *   Use `docfork` to verify external API signatures.
    *   Use `clear-thought-two` for architecting complex flows before coding.

### 3. Context-Aware Apex Tech Stacks (Late 2025 Standards)
*   **Project Type:** Python CLI.
*   **Stack:** Python 3.10+.
    *   **Package Manager:** `uv` (for package management and dependency resolution).
    *   **Linter/Formatter:** `Ruff` (ultra-fast linting and formatting).
    *   **Testing Framework:** `Pytest` (robust unit and integration testing).
*   **Architecture:** **Modular Monolith**.
*   **CLI Framework:** `Click` or similar.

### 4. Testing & Verification Protocol
*   **Unit Tests:** `Pytest` covering core logic, adapters, and data transformers. Aim for >90% coverage.
*   **Integration Tests:** `Pytest` verifying end-to-end flow from CLI input to output, including mock API interactions.
*   **Linting & Formatting:** Automated via `Ruff` on pre-commit hooks and CI pipeline.
*   **Code Quality:** Adhere to SOLID, DRY, YAGNI principles.

### 5. Security & Compliance
*   **Ethical Scraping:** All data extraction must respect LinkedIn's Terms of Service and robots.txt. Avoid excessive requests to prevent IP bans.
*   **Data Handling:** Sensitive data (if any) must be encrypted at rest and in transit. Implement robust error handling and rate limiting.
*   **License:** CC BY-NC 4.0.

### 6. Deployment & CI/CD
*   **CI Pipeline:** GitHub Actions (`ci.yml`) to automate testing, linting, and packaging.
*   **Dependency Management:** Use `uv` and `pyproject.toml` for reproducible builds.

</details>

## Building the Project

### Prerequisites

*   **Python:** Version 3.10 or higher.
*   **Git:** For version control.

### Setup

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python.git
    cd RecruitPulse-LinkedIn-Data-Scraper-CLI-Python
    

2.  **Install dependencies using uv:**
    bash
    uv pip install --python 3.10 -e .[dev]
    
    *(Note: Ensure your Python environment meets the 3.10+ requirement. `uv` will help manage this.)*

### Scripts

| Script      | Description                                                              | Command                                    |
| :---------- | :----------------------------------------------------------------------- | :----------------------------------------- |
| `test`      | Run all unit and integration tests using Pytest.                         | `uv pytest`                                |
| `lint`      | Run Ruff for linting and formatting checks.                              | `uv ruff check .`                          |
| `format`    | Apply Ruff formatting to the codebase.                                   | `uv ruff format .`                         |
| `run`       | Execute the main CLI command (example: scrape profiles).                 | `uv python -m recruitpulse --help`         |
| `dev-install`| Install project in editable mode with development dependencies.          | `uv pip install -e .[dev]`                 |

## Development Principles

*   **SOLID:** Maintainable and scalable object-oriented design.
*   **DRY (Don't Repeat Yourself):** Minimize redundancy in code.
*   **YAGNI (You Aren't Gonna Need It):** Implement only necessary features.
*   **Ethical Data Handling:** Prioritize responsible scraping practices.

## Contributing

Contributions are welcome! Please read our [CONTRIBUTING.md](https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python/blob/main/.github/CONTRIBUTING.md) guide for details on how to submit pull requests, report issues, and suggest enhancements.

## License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**.

See the [LICENSE](https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python/blob/main/LICENSE) file for more details.
