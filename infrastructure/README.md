## 🏗️ **infrastructure/** Module

### 🌐 **Purpose:**
The `infrastructure` folder provides repositories and tools focused on setting up, managing, and automating deployment environments. This module ensures the scalability, security, and reliability of applications through DevOps practices, CI/CD pipelines, and infrastructure management solutions.

---

### 📚 **What You Can Find Here:**
- 🚀 **Deployment Tools:** Repositories for automating server provisioning, application deployment, and scaling.
- 🔐 **Authentication and Security Services:** Tools and libraries to secure applications, manage access control, and handle user authentication.
- ⚙️ **Configuration Management:** Solutions for managing and maintaining configuration files across environments.
- 🔄 **CI/CD Pipelines:** Continuous integration and deployment setups for automated builds and testing.

---

### 👨‍💻 **Developer Contribution Opportunities:**
- 🚀 **Enhance Deployment Automation:** Contribute scripts or tools to optimize infrastructure provisioning and scaling.
- 🔐 **Improve Security Services:** Add new authentication methods, access control mechanisms, or vulnerability scanners.
- 🛠 **Optimize CI/CD Pipelines:** Help improve build processes, automated testing, and continuous delivery.
- 📖 **Documentation:** Provide guides on infrastructure best practices, deployment workflows, or environment setup.

For more details on contributing, please refer to the [CONTRIBUTING.md](./CONTRIBUTING.md) file. Let’s build resilient and scalable infrastructure together! 🌟

# Capabilities of File Service

### Flexible integration with cloud storage

- Support for S3 (Amazon, MinIO), DigitalOcean Spaces, etc.
- Local disk (in development environments or if there is no cloud).
- Developers don’t need to set up integration themselves — File Service already knows how to store and serve files via URL.

### Document generation from templates

- Django-template (or similar) logic inside, support for PDF/PNG.
- Automatic data substitution from JSON.
- Can cover many use cases for generating acts, invoices, contracts "on the fly."

### Soft deletion mechanism

- When a file is deleted, a `deleted=true` flag is set.
- There is a periodic/manual mechanism for final cleanup (`cleanup`).

Useful for "safe" deletion and the possibility of "restoration" if needed.

