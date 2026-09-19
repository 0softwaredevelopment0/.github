# Security Policy

The **0softwaredevelopment0** organization takes security seriously. We appreciate your efforts to responsibly disclose vulnerabilities.

---

## Supported Versions

Security updates are provided for the **latest release** of each project.

| Project | Supported |
|---------|-----------|
| RustLauncher | Latest release |
| SoundPad | Latest release |
| IpParser | Latest release |
| OrganizationWebsite | Always running latest |
| All other projects | Latest release |

---

## Reporting a Vulnerability

**Do NOT open a public Issue for security vulnerabilities.**

If you discover a security vulnerability, please report it **privately** via one of the following methods:

### Option 1: Email (Preferred)

Send an email to: **[dan.al.zhu@gmail.com](mailto:dan.al.zhu@gmail.com)**

Include:
- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Suggested fix (if any)

### Option 2: GitHub Security Advisories

Use [GitHub's private vulnerability reporting](https://github.com/0softwaredevelopment0) → Security tab → "Report a vulnerability" in the affected repository.

---

## What to Include

When reporting a vulnerability, please provide:

1. **Type of vulnerability** (e.g., remote code execution, SQL injection, XSS, DoS, path traversal)
2. **Affected project and version**
3. **Steps to reproduce** (proof of concept if possible)
4. **Impact assessment** — what could an attacker achieve?
5. **Suggested mitigation** — if you have ideas for fixing it

---

## Response Timeline

| Action | Timeline |
|--------|----------|
| Acknowledgment of report | Within **48 hours** |
| Initial assessment | Within **1 week** |
| Fix or mitigation | Within **2-4 weeks** depending on severity |
| Public disclosure | After fix is released |

---

## Disclosure Policy

- We follow **responsible disclosure** — please do not publicly disclose the vulnerability until a fix is available.
- We will credit reporters in the release notes (unless you prefer to remain anonymous).
- We will not take legal action against researchers who follow this policy.

---

## Security Best Practices for Contributors

When contributing code to our projects:

- **Never commit secrets** (API keys, passwords, tokens) to the repository.
- Use **environment variables** or **config files** (gitignored) for sensitive data.
- Validate and sanitize all user inputs.
- Use prepared statements for database queries.
- Follow the principle of **least privilege**.
- Keep dependencies up to date.

---

## Resources

- [GitHub Security Advisories](https://docs.github.com/en/security/advisories)
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [AGPLv3 License](https://www.gnu.org/licenses/agpl-3.0.html)

---

Thank you for helping keep our projects and users safe!
