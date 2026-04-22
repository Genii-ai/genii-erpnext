# Genii ERPNext

Custom ERPNext modules for factory-built housing development.

## Stack
- ERPNext v16.10.1, Frappe Framework
- Docker Compose at erp.geniinow.com
- Python server-side, JS client-side (Vue.js within Frappe)

## Patterns
- Custom doctypes in `genii_crm/` app
- API needs User-Agent header to bypass Cloudflare 403
- Base URL: https://erp.geniinow.com
- Use `frappe.get_doc()` and `frappe.db.sql()` for data access
- Client scripts in `public/js/`, server in `api.py`
- Never commit credentials
