# How Broken Access Control Happens

Broken access control is rarely caused by missing authentication.  
It is caused by **incorrect authorization logic**.

## Common Causes

- Trusting client-side role checks
- Missing authorization checks on backend APIs
- Inconsistent access logic across microservices
- Hardcoded roles instead of policy-based access
- Over-reliance on UI restrictions

## Key Insight

> Authentication answers **who you are**  
> Authorization answers **what you can do**

Most systems fail at the second question.
