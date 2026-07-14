---
title: "Password requirements"
weight: 20
---

When you create a virtual machine, you set a password for the administrator account. Follow these rules to avoid creation errors.

## Rules

| Requirement | Value |
|-------------|-------|
| Minimum length | 12 characters |
| Maximum length | 128 characters |
| Uppercase letters | At least 1 (A–Z) |
| Lowercase letters | At least 1 (a–z) |
| Numbers | At least 1 (0–9) |
| Special characters | At least 1 (`!@#$%^&*()_+-=[]{}|;:,.<>?`) |

## Examples

| Password | Result | Why |
|----------|--------|-----|
| `MyStrongPass2026!` | ✅ Accepted | Meets all rules |
| `short1A!` | ❌ Rejected | Too short (8 characters, need 12) |
| `alllowercase123!` | ❌ Rejected | No uppercase letter |
| `NoNumbersHere!` | ❌ Rejected | No digit |

## If you forget the password

You cannot recover the password of an existing VM. If you lose it, you have two options:

1. **Recreate the VM** with a new password.
2. **Use the WebConsole** if you still have an active session.

**Warning:** Recreating the VM deletes all data on it. Back up your files before you delete a VM.

---

**Related pages:**

- [Create a virtual machine](../../../02-basics/01-create-vm/)
- [Troubleshooting login issues](../../../04-troubleshoot/)
