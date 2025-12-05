# Security Policy

## Supported Versions

We actively support and provide security patches for the following versions of RecruitPulse-LinkedIn-Data-Scraper-CLI-Python:

| Version | Supported          |
| ------- | ------------------ |
| Latest  | :white_check_mark: |


## Reporting a Vulnerability

We take the security of our project seriously. If you find a security vulnerability, please report it promptly via one of the methods below. We will promptly investigate and take appropriate action.

**DO NOT** disclose the vulnerability publicly until it has been fixed and communicated by the project maintainers.

### Reporting Channels

1.  **GitHub Security Advisory:** The preferred method is to submit a security advisory directly through GitHub. Please go to `https://github.com/chirag127/RecruitPulse-LinkedIn-Data-Scraper-CLI-Python/security/advisories` to create a new advisory.
2.  **Email:** You can also send an encrypted email to `chirag.dev@example.com` (replace with actual secure email if available). Please use PGP/GPG encryption if possible. If you do not have PGP, we will still investigate unencrypted reports, but please be aware of the risks.

### Information to Include

When reporting a vulnerability, please include as much of the following information as possible:

*   **Vulnerability Type:** (e.g., Cross-Site Scripting (XSS), SQL Injection, Broken Authentication, etc.)
*   **Affected Component(s):** Specify the part of the project that is vulnerable.
*   **Steps to Reproduce:** Provide clear, step-by-step instructions to reproduce the vulnerability.
*   **Impact:** Describe the potential consequences if the vulnerability is exploited.
*   **Suggested Mitigation (Optional):** If you have ideas on how to fix the vulnerability, please include them.

## Security Team Response

*   We will acknowledge receipt of your vulnerability report within **48 hours**.
*   We will aim to provide an update on the status of the vulnerability investigation and any planned remediation within **7 days**.
*   We will disclose the vulnerability publicly after it has been fixed and released to users, crediting the reporter.

## Security Best Practices

As a Python CLI tool, users should adhere to general security best practices when using and developing with RecruitPulse-LinkedIn-Data-Scraper-CLI-Python:

*   **Environment Security:** Ensure your Python environment is secure and up-to-date. Use virtual environments (`uv` is recommended for this project) to isolate dependencies.
*   **Dependency Management:** Regularly update dependencies using `uv`. Be cautious when adding new dependencies.
*   **Data Handling:** Be mindful of the data you are scraping and how you store and process it. Ensure compliance with relevant data privacy regulations.
*   **API Keys and Credentials:** If the tool interacts with external APIs that require authentication, handle API keys and credentials securely. Do not hardcode them directly in scripts; use environment variables or secure configuration management.
*   **Code Reviews:** For any contributions or modifications, ensure thorough code reviews are conducted, focusing on security implications.

Thank you for helping to keep RecruitPulse-LinkedIn-Data-Scraper-CLI-Python secure!
