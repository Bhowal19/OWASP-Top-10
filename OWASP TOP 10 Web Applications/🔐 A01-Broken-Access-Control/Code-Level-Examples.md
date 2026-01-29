# Code-Level Examples

## Insecure Pattern

```javascript
if (user.isAuthenticated) {
  return getUserData(requestedUserId);
}

Secure Pattern

if (user.id === requestedUserId || user.role === 'admin') {
  return getUserData(requestedUserId);
}

Key Takeaway

- Authorization must be:
- Explicit
- Centralized
- Enforced server-side

