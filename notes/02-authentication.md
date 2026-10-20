# Authentication & Session Management

**Confidence:** 🟡 review

## Key concepts
- **AuthN vs AuthZ** — who you are vs. what you're allowed to do.
- **Session cookies vs. tokens** (JWT/opaque) — tradeoffs in revocation and storage.
- **OAuth 2.0 / OIDC** — delegated authorization; **PKCE** protects public clients against auth-code interception (I implemented OAuth 2.0 + PKCE during my Advantive internship).
- **MFA** factors and why phishing-resistant (FIDO2/WebAuthn) matters.

## Common weaknesses (and the defense)
- Weak password storage → use a slow, salted KDF (bcrypt/argon2).
- Predictable session IDs → use CSPRNG, rotate on privilege change.
- Missing logout / session fixation → invalidate server-side on logout and after auth.

## Questions to be able to answer
- What exactly does PKCE prevent, and why do SPAs need it?
- Where should a JWT live in the browser, and what's the XSS vs CSRF tradeoff?

## My notes
_Fill in._
