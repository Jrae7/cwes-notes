# Web Security Fundamentals

**Confidence:** 🟡 review

## Key concepts
- **HTTP(S) request/response lifecycle** — methods, status codes, headers, cookies.
- **Same-Origin Policy (SOP)** and how **CORS** selectively relaxes it.
- **TLS** — what it protects (confidentiality, integrity, server identity) and what it does not (it doesn't fix app-layer bugs).
- **Statelessness** — HTTP is stateless; sessions/tokens add state.

## Core security headers (defense)
| Header | Purpose |
|--------|---------|
| `Content-Security-Policy` | Mitigates XSS by restricting script sources |
| `Strict-Transport-Security` | Forces HTTPS |
| `X-Content-Type-Options: nosniff` | Stops MIME sniffing |
| `Set-Cookie` flags `HttpOnly`, `Secure`, `SameSite` | Protects session cookies |

## Questions to be able to answer
- Why can't TLS alone stop an injection attack?
- What does `SameSite=Lax` vs `Strict` change for CSRF?

## My notes
_Add examples observed in the lab here._
