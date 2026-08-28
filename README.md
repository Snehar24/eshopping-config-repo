# EShoppingZone Config Repository

This repository contains environment-safe Spring Cloud Config files for EShoppingZone. Do not commit passwords, API keys, SMTP credentials, or database credentials. They are supplied through environment variables.

## Publish to GitHub

Create a private GitHub repository named `eshoppingzone-config`, push this folder to its `main` branch, then start `config-server` with:

```powershell
$env:CONFIG_SERVER_PROFILE = "git"
$env:CONFIG_REPOSITORY_URI = "https://github.com/YOUR_USERNAME/eshoppingzone-config.git"
```

For notification emails, configure these environment variables in the environment where `storefront` runs:

```powershell
$env:MAIL_ENABLED = "true"
$env:MAIL_HOST = "smtp.example.com"
$env:MAIL_PORT = "587"
$env:MAIL_USERNAME = "your-smtp-user"
$env:MAIL_PASSWORD = "your-app-password"
$env:MAIL_FROM = "orders@your-domain.com"
```
