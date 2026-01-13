# Solus Recipes 🐧

A collection of custom `package.yml` recipes for **Solus OS**. These recipes are either not available in the official repositories or have been modified to improve user experience and system integration.

## 📦 Included Recipes

### 1. CUPS-PDF (v3.0.2)
A PDF printer backend for CUPS.
* **Custom Fixes:** * Correctly configured for the Solus `lp` group (no `cups` group errors).
    * Output directory set to `${HOME}/PDF` for easy access.
    * Clean configuration file (no duplicated `Out` directives).
    * Proper SUID permissions for seamless file generation in the user's home.

### 2. Pix (v3.4.10)
An advanced image management application.
* Updated to version 3.4.10 (ahead of official repo).

---

## 🛠️ How to build and install

To use these recipes, you need to have the development tools installed on your Solus system.

### Prerequisites
Install the packaging tools:
```bash
sudo eopkg install-repo -is ypkg solbuild
