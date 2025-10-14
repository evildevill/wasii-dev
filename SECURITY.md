# Security Policy

## 🔒 Security at wasii.dev

As a cybersecurity professional's personal portfolio and educational platform, we take security seriously and appreciate the community's help in keeping the platform safe.

---

## 🛡️ Reporting Security Vulnerabilities

**DO NOT** open public issues for security vulnerabilities.

### How to Report

Please report security issues privately to:

- **Primary**: hi@wasii.dev
- **Alternative**: support@wasii.dev
- **Subject Line**: "[SECURITY] Brief Description"

### What to Include

1. **Summary** - One-sentence description
2. **Impact** - What could an attacker do?
3. **Steps to Reproduce** - Detailed reproduction steps
4. **Proof of Concept** - Code or screenshots (if safe)
5. **Suggested Fix** - If you have one (optional)
6. **Disclosure Timeline** - Your preferred timeline

### Example Report

```
Subject: [SECURITY] Potential XSS in Comment System

Summary: Unescaped user input in comments allows XSS attacks

Impact: Attackers can execute JavaScript in other users' browsers

Steps to Reproduce:
1. Navigate to any blog post
2. Post comment with: <script>alert('XSS')</script>
3. Page executes the script

Suggested Fix: Use DOMPurify to sanitize comment HTML before rendering
```

---

## ⏱️ Response Timeline

| Phase | Target Time |
|-------|-------------|
| Acknowledgment | Within 48 hours |
| Initial Triage | Within 5 business days |
| Fix or Plan | Within 30 days (critical/high) |
| Deployment | As soon as tested |
| Public Disclosure | After fix or by mutual agreement |

---

## 🎯 In Scope

Security issues in these areas are in scope:

✅ **Authentication & Authorization**
- Login/logout flows
- Session management
- Access control bypasses
- Permission escalation

✅ **Data Security**
- SQL/NoSQL injection
- Sensitive data exposure
- Insecure data storage
- PII leakage

✅ **Web Vulnerabilities**
- XSS (Cross-Site Scripting)
- CSRF (Cross-Site Request Forgery)
- SSRF (Server-Side Request Forgery)
- Path traversal
- Open redirects

✅ **API Security**
- API authentication bypass
- Rate limiting issues (if exploitable)
- Mass assignment vulnerabilities
- Insecure direct object references (IDOR)

✅ **File Upload Issues**
- Malicious file upload
- File type validation bypass
- Path traversal via filename

✅ **Business Logic Flaws**
- Payment bypass
- Free premium access
- Unauthorized course access
- Certificate forgery

---

## ⛔ Out of Scope

The following are **not** considered security issues:

- ❌ Denial of Service (DoS/DDoS) attacks
- ❌ Social engineering attacks
- ❌ Physical attacks
- ❌ Issues in third-party services (Kinde, Vercel, MongoDB Atlas)
- ❌ Missing security headers (unless exploitable)
- ❌ Missing rate limiting (unless exploitable)
- ❌ Self-XSS (requires user to paste malicious code)
- ❌ Clickjacking on non-sensitive pages
- ❌ Descriptive error messages (unless leaking secrets)
- ❌ Automated vulnerability scanner output without PoC
- ❌ Issues requiring compromised devices or stolen credentials

---

## 🏆 Recognition

Researchers who responsibly disclose vulnerabilities may be:

- Listed in our Hall of Fame (with permission)
- Acknowledged in security advisories
- Given credit in release notes

### Hall of Fame

*No security researchers yet. Be the first!*

---

## 🛡️ Current Security Measures

The platform implements:

- ✅ HTTPS enforcement with HSTS
- ✅ Secure authentication (Kinde Auth)
- ✅ Input validation (Zod schemas)
- ✅ Security headers (X-Frame-Options, X-Content-Type-Options)
- ✅ CSRF protection (SameSite cookies)
- ✅ File upload validation (type, size)
- ✅ Rate limiting on sensitive endpoints
- ✅ Audit logging for admin actions
- ✅ Webhook signature verification
- ✅ Parameterized database queries
- ✅ Environment variable protection
- ✅ Dependency vulnerability scanning

---

## 🔍 Vulnerability Disclosure Policy

We follow coordinated disclosure:

1. You report the issue privately
2. We acknowledge and investigate
3. We develop and test a fix
4. We deploy the fix to production
5. We notify affected users (if needed)
6. We publicly disclose (with your permission)

---

## 📜 Safe Harbor

When researching security issues:

✅ **DO:**
- Use test accounts only
- Report findings promptly
- Provide detailed reproduction steps
- Act in good faith

❌ **DON'T:**
- Access other users' data
- Perform attacks that degrade service
- Share vulnerabilities publicly before fix
- Demand payment or rewards

If you follow these guidelines, we will not pursue legal action.

---

## 🔐 Encryption

We support encrypted communication:

- Email encryption available on request
- PGP key: (Available on request at hi@wasii.dev)

---

## 📚 Security Resources

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [CWE Top 25](https://cwe.mitre.org/top25/)
- [Next.js Security](https://nextjs.org/docs/app/building-your-application/configuring/security)

---

## 🤝 Thank You

Thank you for helping keep wasii.dev secure for everyone!

---

**Last Updated**: October 2025
