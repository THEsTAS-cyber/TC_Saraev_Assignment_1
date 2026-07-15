---
title: "Troubleshooting"
weight: 70
---

## Troubleshooting

This section helps you diagnose and resolve common issues with Innopolis VM. Each problem follows a structured approach: **Symptom**, **Possible causes**, **Checks**, **Solutions**, and **Escalation**.

---

### Gray screen — cannot click anything

**Symptom:**  
The screen turned gray and you cannot interact with the interface.

**Possible causes:**
- Your session has timed out due to inactivity.
- The browser lost connection to the server.
- The browser tab is unresponsive.

**Checks:**
1. Look at the bottom of the screen for a message like «Your session timed out. Click **OK** to log in again».
2. Check your internet connection.

**Solutions:**
1. Click **OK** in the message.
2. Log in again with your Innopolis University credentials.
3. If the message does not appear, refresh the browser page.

**Escalation:**  
If the problem persists after refreshing and logging in again, contact the IT department of Innopolis University.

---

### Subscription is syncing for too long

**Symptom:**  
Your subscription has been in the «Syncing» status for more than 10 minutes.

**Possible causes:**
- Normal synchronization delay with the SSO system.
- Temporary server-side processing.
- An issue with your account permissions.

**Checks:**
1. Check the current status of your subscription on the **My Account** → **SUBSCRIPTIONS** page.
2. Try to create a VM — if it works, the subscription is already active despite the «Syncing» label.

**Solutions:**
1. Wait 10–15 minutes. In most cases, the status will change to «Active» automatically.
2. Try using the subscription — it is likely already active.

**Escalation:**  
If the subscription remains in «Syncing» status for more than 30 minutes, contact the IT department of Innopolis University.

---

### VM is creating for too long

**Symptom:**  
Your VM has been in the «Creating» status for more than 15 minutes.

**Possible causes:**
- High load on the Innopolis VM servers.
- Insufficient resources in your subscription.
- A template configuration error.

**Checks:**
1. Check the VM status on the **VIRTUAL MACHINES** page.
2. Wait at least 15 minutes — some templates take longer to provision.

**Solutions:**
1. Delete the stuck VM.
2. Create a new VM with the same settings.

**Escalation:**  
If you have tried to recreate the VM 2–3 times and it still fails, contact the IT department of Innopolis University.

---

### VM failed to create

**Symptom:**  
You received an error message during VM creation.

**Possible causes:**
- Incorrect password (does not meet requirements).
- Insufficient resources in your subscription.
- A template or configuration error.

**Checks:**
1. Click the **i** button next to the failed VM to see the error details.
   ![Failed to create message](../../../en/images/Failed_to_create_message.png)
2. Review the error message for specific clues.

**Solutions:**
1. Fix the issue described in the error message (e.g., change the password to meet requirements).
2. Delete the failed VM and create a new one with corrected settings.

**Escalation:**  
If the error persists after 2–3 attempts with corrected settings, contact the IT department of Innopolis University.

---

### Forgot account password

**Symptom:**  
You cannot log in to Innopolis VM with your Innopolis University credentials.

**Possible causes:**
- You forgot your password.
- Incorrect keyboard layout or Caps Lock is on.
- Your account is locked or deactivated.

**Checks:**
1. Verify your keyboard layout and make sure Caps Lock is off.
2. Try logging in at `sso.university.innopolis.ru` directly.

**Solutions:**
1. Use the «Forgot password» option on the SSO login page to reset your password.
2. Log in again with the new password.

**Escalation:**  
If you cannot reset your password or your account is locked, contact the IT department of Innopolis University.

---

### Forgot VM password

**Symptom:**  
You cannot log in to your VM via SSH or WebConsole.

**Possible causes:**
- You forgot the password you set during VM creation.
- Incorrect keyboard layout or Caps Lock is on.
- The password was changed by another administrator.

**Checks:**
1. Verify your keyboard layout and make sure Caps Lock is off.
2. Try the default logins: `root`, `admin`, or `administrator` (depending on the OS).
3. Check if you still have an active WebConsole session.

**Solutions:**

> **Warning:** Recreating a VM permanently deletes all data on it. Back up your files before proceeding.

If you cannot recover the password, you have two options:
1. **Use the WebConsole** if you still have an active session — you can change the password from inside the VM.
2. **Recreate the VM** with a new password.

**Escalation:**  
If you need to recover data from a VM with a lost password, contact the IT department of Innopolis University immediately — they may be able to help before the VM is deleted.