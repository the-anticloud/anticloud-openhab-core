# How to Update — OPENHAB_CORE

**Project:** `OPENHAB_CORE`
**Category:** CONSUMER_APPLIANCES
**Domain:** consumer appliances and IoT
**Date:** 2026-10-07

---

## Update Procedure

### Checking for Updates
```bash
OPENHAB_CORE --version
OPENHAB_CORE check-update
```

### Applying Updates
```bash
pip install --upgrade OPENHAB_CORE
```

### Rolling Back
```bash
pip install OPENHAB_CORE==<previous-version>
```

### Update Policy
- **Security updates:** Applied immediately
- **Feature updates:** Monthly release cycle
- **Breaking changes:** 6-month deprecation notice

## Verification

All 16 checks PASS. Evidence: `ISOLATED_LAB_RESULTS/03_Result_Register.md`.
