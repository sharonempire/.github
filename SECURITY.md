# Security Policy

## Reporting a Vulnerability

If you discover a security vulnerability in any Codnov repository, please report it responsibly.

**Do NOT open a public GitHub issue for security vulnerabilities.**

Instead, email: **nidin@codnov.ai**

Include:
- Description of the vulnerability
- Steps to reproduce
- Affected repository and version
- Potential impact

We will acknowledge receipt within 48 hours and provide a fix timeline.

## Supported Versions

Only the latest version on the `main` branch of each repository is supported with security updates.

## Security Practices

- All secrets are stored in environment variables, never in code
- Authentication tokens use httpOnly cookies (web) or SecureStore (mobile)
- All API communication is over HTTPS
- Dependencies are monitored for known vulnerabilities
- Code review is required for all changes to `main`
