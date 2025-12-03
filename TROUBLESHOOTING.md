# VS Code Usage Limit Troubleshooting Guide

## Issue: "I have paid but VS Code says I've reached my usage limit"

If you're seeing a usage limit message in VS Code even after upgrading to Pro or making a payment, this guide will help you resolve the issue.

## Common Causes and Solutions

### 1. Subscription Not Yet Synced
**Symptom:** Just upgraded/paid but still seeing usage limits

**Solution:**
- Wait 5-10 minutes after payment for the subscription to sync
- Restart VS Code completely (close all windows)
- Sign out and sign back in to your GitHub/Microsoft account in VS Code
  - Go to: Settings → Accounts → Sign out
  - Then sign back in with the account that has the Pro subscription

### 2. Wrong Account Logged In
**Symptom:** Multiple accounts and not sure which one has the subscription

**Solution:**
- Check which account is currently active in VS Code
- Verify your subscription at: https://github.com/settings/copilot
- Ensure VS Code is signed in with the same account that has the active subscription
- If using GitHub Copilot, check: https://github.com/settings/copilot

### 3. Extension Needs Update
**Symptom:** Using an older version of the extension

**Solution:**
- Update all VS Code extensions to the latest version
- Check for VS Code updates: Help → Check for Updates
- Specifically update: GitHub Copilot, GitHub Copilot Chat extensions
- Restart VS Code after updates

### 4. Cache Issues
**Symptom:** Subscription shows active but VS Code doesn't recognize it

**Solution:**
- Clear VS Code cache:
  - Close VS Code completely
  - Delete cache folders (backup first if unsure):
    - Windows: `%APPDATA%\Code\Cache`, `%APPDATA%\Code\CachedData`
    - macOS: `~/Library/Application Support/Code/Cache`
    - Linux: `~/.config/Code/Cache`
- Restart VS Code and sign in again

### 5. Verify Subscription Status

**Steps to verify:**
1. Go to your GitHub account settings
2. Navigate to Copilot settings: https://github.com/settings/copilot
3. Confirm your subscription is active
4. Check billing: https://github.com/settings/billing
5. Ensure payment was processed successfully

### 6. Network/Proxy Issues
**Symptom:** Connection issues preventing license verification

**Solution:**
- Check your internet connection
- If behind a corporate proxy, ensure it allows GitHub/Microsoft authentication
- Temporarily disable VPN to test
- Check firewall settings

## Step-by-Step Troubleshooting

1. **Verify Payment Processed**
   - Check your email for payment confirmation
   - Check credit card/payment method for charge
   - Visit GitHub billing to confirm active subscription

2. **Force Refresh in VS Code**
   - Press Ctrl+Shift+P (Cmd+Shift+P on Mac)
   - Type: "Developer: Reload Window"
   - Press Enter

3. **Sign Out and Sign In**
   - In VS Code, click on account icon (bottom left)
   - Sign out from all accounts
   - Sign in again with your Pro account
   - Grant all requested permissions

4. **Check Extension Status**
   - Open Extensions view (Ctrl+Shift+X)
   - Search for your extension (e.g., "GitHub Copilot")
   - Verify it's installed and enabled
   - Check for updates

5. **Contact Support**
   - If issue persists after trying above steps
   - GitHub Support: https://support.github.com/
   - VS Code Issues: https://github.com/microsoft/vscode/issues
   - Include:
     - Account email
     - Payment confirmation
     - Screenshots of the error
     - VS Code version
     - Extension versions

## Quick Reference Commands

### VS Code Command Palette (Ctrl+Shift+P / Cmd+Shift+P)

- `Developer: Reload Window` - Refresh VS Code
- `GitHub Copilot: Sign Out` - Sign out of Copilot
- `GitHub Copilot: Sign In` - Sign in to Copilot
- `Extensions: Check for Extension Updates` - Update extensions

## Additional Resources

- GitHub Copilot Documentation: https://docs.github.com/en/copilot
- VS Code Documentation: https://code.visualstudio.com/docs
- GitHub Support: https://support.github.com/
- GitHub Billing Help: https://docs.github.com/en/billing

## Still Having Issues?

If you've tried all the above steps and still experiencing issues:

1. **Document the Issue:**
   - Take screenshots of error messages
   - Note your VS Code version (Help → About)
   - Note extension versions
   - Copy any error messages from Developer Console (Help → Toggle Developer Tools)

2. **Contact Support:**
   - For GitHub Copilot: https://support.github.com/
   - For VS Code: https://github.com/microsoft/vscode/issues
   - For other extensions: Check extension's repository issues page

3. **Provide Details:**
   - Your account email (that has the subscription)
   - Payment confirmation number/date
   - Exact error message
   - Steps you've already tried
   - Your system (Windows/Mac/Linux)

---

**Note:** Most subscription sync issues resolve within 10-15 minutes of payment processing. If it's been longer than an hour, follow the troubleshooting steps above.
