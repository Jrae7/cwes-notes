# Access Control

**Confidence:** 🔴 not yet covered

## Key concepts
- Models: **RBAC**, **ABAC**, **MAC/DAC** — when each fits.
- **IDOR / BOLA** — authorization checks that rely on the client not to tamper with object references.
- **Privilege escalation** — horizontal vs. vertical.
- **Principle of least privilege** and default-deny.

## Defense checklist
- Enforce authorization **server-side on every request**, keyed to the authenticated identity.
- Check ownership of the specific object, not just that the user is logged in.
- Centralize authorization logic rather than scattering checks.

## Questions to be able to answer
- Why is a hidden/disabled UI control not an access control?
- How would a detection rule catch repeated authorization failures? (ties to my [`wazuh-detections`](https://github.com/Jrae7/wazuh-detections))

## My notes
_Fill in._
