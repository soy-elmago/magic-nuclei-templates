# Nuclei Template – Multilingual User Registration Page (Headless Required)

This is a custom Nuclei template created to detect multilingual user registration pages in web applications.  
It identifies common registration fields such as `full_name`, `email`, `password`, `gender`, and others, across different languages (e.g., English and Spanish).

> ⚠️ **Important:** This template requires the `-headless` flag when running Nuclei, as it relies on DOM-based detection. Without `-headless`, it won't work properly.

## Usage

```bash
nuclei -t user-registration-multilang.yaml -u https://target.com -headless
```
