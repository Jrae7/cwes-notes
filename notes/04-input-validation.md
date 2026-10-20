# Input Validation & Injection

**Confidence:** 🔴 not yet covered

## Key concepts
- Injection happens when **untrusted input is interpreted as code/commands** (SQL, OS, template, LDAP, etc.).
- **XSS** — reflected, stored, DOM-based; the fix is context-aware output encoding + CSP.
- **Validation vs. encoding vs. parameterization** — different tools for different stages.

## Defense checklist
- **Parameterized queries / prepared statements** for data access (not string concatenation).
- **Output encoding** at the point of use, matched to the context (HTML, attribute, JS, URL).
- **Allowlist validation** of structure/type/length where feasible.
- Treat all client-supplied data as untrusted, including headers and cookies.

## Questions to be able to answer
- Why does parameterization stop SQL injection where escaping often fails?
- What makes DOM-based XSS different to detect server-side?

## My notes
_Fill in. Study any hands-on examples only in the authorized lab._
