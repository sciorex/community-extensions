# Security Policy

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| 1.x.x   | :white_check_mark: |

## Reporting a Vulnerability

We take security seriously. If you discover a security vulnerability in any community agent or flow, please report it responsibly.

### How to Report

**Do not create a public issue for security vulnerabilities.**

Instead, please email us at: **security@sciorex.com**

Include the following information:

1. **Agent/Flow affected**: Name and version
2. **Description**: Clear description of the vulnerability
3. **Impact**: What could an attacker do with this vulnerability?
4. **Steps to reproduce**: Detailed steps to reproduce the issue
5. **Suggested fix**: If you have one

### What to Expect

- **Acknowledgment**: We will acknowledge your report within 48 hours
- **Investigation**: We will investigate and provide updates within 7 days
- **Resolution**: We aim to fix confirmed vulnerabilities within 30 days
- **Credit**: With your permission, we will credit you in the security advisory

### Security Considerations for Contributors

When contributing agents or flows, please ensure:

1. **No hardcoded secrets**: Never include API keys, tokens, or credentials
2. **Minimal permissions**: Request only the tools your agent needs
3. **Input validation**: Validate inputs in your system prompts
4. **Safe outputs**: Don't generate code that could be harmful
5. **No data exfiltration**: Agents should not send data to external services

### Safe Tool Usage

Be cautious with tools that can modify the system:

| Tool | Risk Level | Guidance |
|------|------------|----------|
| `Read` | Low | Generally safe |
| `Glob` | Low | Generally safe |
| `Grep` | Low | Generally safe |
| `Write` | Medium | Be careful about file paths |
| `Edit` | Medium | Validate before editing |
| `Bash` | High | Limit to specific commands |

### Review Process

All submitted agents and flows undergo review for:

- Malicious code patterns
- Excessive permissions
- Data privacy concerns
- Security best practices

## Security Updates

Security updates will be released as patch versions (e.g., 1.0.0 → 1.0.1) and announced in:

- GitLab Security Advisories
- Repository releases
- Discord announcements

## Questions

For general security questions, please open an issue at [GitLab Issues](https://gitlab.com/sciorex/community-extensions/-/issues).
