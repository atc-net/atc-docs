# Security

- ✔️ **Do** limit the deployment Application   Identity access to resources on the environments
    > *Always follow the Principle of Least Privilege when granting access to resources.*
- ✔️ **Do** require HTTPS/TLS 1.2 as a minimum
- ✔️ **Do** protect your API/App transport with SSL
- ✔️ **Do** protect and restrict API/App access with OAuth2 through e.g. Azure AD
- ✔️ **Do** protect your data at rest with encryption
- ✔️ **Do** use role-based access control where possible
- ✔️ **Do** use a secret store for storing application secrets - e.g. Azure Key Vault
- ❌ **Do not** keep secrets in source- and automation code
    > *Sensitive information like password, tokens and keys must be stored securely encrypted for security and maintainability. Azure Key Vault is good candidate for this.*
- ❌ **Do not** invent your own custom security implementation, but use industry standards
