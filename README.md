# Magic Nuclei Templates

This repository contains a collection of custom [Nuclei](https://github.com/projectdiscovery/nuclei) templates created to assist in reconnaissance, vulnerability detection, and web application analysis.

Each template is handcrafted to target specific patterns, misconfigurations, or endpoints that may be useful for bug bounty hunting or pentesting.

---

## Available Templates

### 📝 `user-registration-multilang.yaml`

Detects multilingual user registration pages in web applications by identifying fields such as `full_name`, `email`, `password`, `gender`, etc., in multiple languages (e.g., English and Spanish).

> ⚠️ **Requires the `-headless` flag**, as it uses DOM-based matchers. Without `-headless`, the template will not function correctly.

**Usage:**

```bash
nuclei -t user-registration-multilang.yaml -u https://target.com -headless
```
