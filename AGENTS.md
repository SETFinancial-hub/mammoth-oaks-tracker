# Codex Agent Guidelines

## Review guidelines

- Flag security vulnerabilities as P0 (authentication bypasses, SQL injection, XSS, exposed secrets/credentials).
- Flag bugs that would cause data loss or incorrect financial calculations as P0.
- Flag missing error handling in API calls, database operations, and external service integrations as P1.
- Flag hardcoded secrets, API keys, or credentials in source code as P0.
- Verify environment variables are used for configuration rather than hardcoded values.
- Check for proper input validation on user-facing endpoints.
- Flag console.log statements that leak sensitive data.
- Treat unhandled promise rejections and missing async/await as P1.
- Ignore stylistic preferences (formatting, naming conventions) unless they cause confusion.
