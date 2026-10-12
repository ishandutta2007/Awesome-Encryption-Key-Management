# Awesome-Encryption-Key-Management

# Top Encryption Key Management Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Cryptographic Key Lifecycle, Secrets Management & Hardware Security*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Encryption Key Management**. These tools enable organizations to generate, store, rotate, and control access to cryptographic keys and secrets — securing data at rest, in transit, and across cloud environments while meeting compliance requirements.

**Examples** include Salesforce Key Management, HashiCorp Vault, AWS KMS, Azure Key Vault, Google Cloud KMS, Akeyless Vault, Fortanix DSM, Thales CipherTrust, Doppler, and CyberArk Conjur (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, hardware security module integration, and open key management — ideal for security engineers, platform teams, and organizations seeking transparent, vendor-independent encryption infrastructure.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Salesforce Key Management](https://help.salesforce.com/)**  
  Salesforce Shield Platform Encryption feature enabling customer-managed keys via Bring Your Own Key (BYOK) or Cache-Only Key Service. Supports key rotation, key destruction, and HSM-backed key storage for compliance requirements.

- **[HashiCorp Vault (HCP)](https://www.hashicorp.com/cloud)**  
  Managed cloud version of Vault. Features namespaces, performance replication, disaster recovery, HSM integration, and FIPS 140-2 builds. Vault Dedicated and HCP Vault available for teams preferring managed operations over self-hosted clusters .

- **[AWS KMS](https://aws.amazon.com/kms/)**  
  Native AWS key management service. Features envelope encryption for virtually every AWS resource, multi-Region keys, XKS (HYOK) for external key control, CloudHSM option, and CloudTrail audit logging. Usage-based pricing per key version and per API call .

- **[Azure Key Vault](https://azure.microsoft.com/en-us/products/key-vault/)**  
  Azure's native key, secret, and certificate service. Features Managed HSM tier (FIPS 140-2 Level 3), Entra RBAC, automatic rotation, and per-operation pricing. Deep integration with Azure ecosystem .

- **[Google Cloud KMS](https://cloud.google.com/security-key-management)**  
  GCP's native key management with Cloud EKM (External Key Manager) for keys residing outside Google entirely. Features Cloud HSM, CMEK across GCP services, key-justification logging, and usage-based pricing .

- **[Akeyless Vault](https://www.akeyless.io/)**  
  SaaS and self-hosted secrets management platform. Features distributed fragments technology, zero-knowledge encryption, dynamic secrets, and PKI. Known for simplified operations compared to Vault .

- **[Fortanix DSM](https://www.fortanix.com/)**  
  Data Security Manager with HSM-as-a-Service. Features FIPS 140-2 Level 3 validated HSMs, key lifecycle management, and multi-cloud key orchestration.

- **[Thales CipherTrust](https://cpl.thalesgroup.com/)**  
  Enterprise key management platform. Features centralized key lifecycle, HSM integration, database encryption, and cloud key management across multi-cloud environments.

- **[Doppler](https://www.doppler.com/)**  
  Developer-first secrets management platform. Features universal secrets management across environments, CLI-driven workflows, and integrations with major cloud providers.

- **[CyberArk Conjur](https://www.conjur.org/)**  
  Enterprise secrets management with open-source core (Conjur OSS under Apache 2.0). Features policy-as-code, machine identity management, and deep integration with CyberArk PAM suite. Conjur Cloud available at approximately $15-40 per authenticating workload per month .

## Open-Source GitHub Projects

- **[HashiCorp Vault](https://github.com/hashicorp/vault)**  
  The de facto standard for open-source secrets management (BSL 1.1 since 2023, with OpenBao fork under MPL 2.0). Features static and dynamic secrets, transit engine for encryption-as-a-service, PKI issuance, transform engine for tokenization, and 15+ auth methods. The only product covering secrets, encryption, and PKI under one operational model. Enterprise editions add namespaces, replication, and HSM support .

- **[OpenBao](https://github.com/openbao/openbao)**  
  Community fork of HashiCorp Vault under MPL 2.0, maintained by the Linux Foundation. Created after Vault's license change to BSL 1.1 in 2023. Preserves the pre-BSL feature set with community governance. API-compatible with Vault, making migration straightforward .

- **[Infisical](https://github.com/Infisical/infisical)**  
  Open-source secrets, certificates, and privileged access management platform (MIT for core, enterprise license for advanced features). 26k+ GitHub stars. Features secrets vaulting, full PKI/certificate authority, KMS for encryption keys, and SSH certificate management. Four secret consumption patterns: SDK runtime fetching, agent-based injection, Kubernetes operator, and platform syncs. Self-hostable via Docker Compose .

- **[Egide](https://github.com/nubster-opensources/egide)**  
  Self-hosted secrets manager in Rust (license varies). Alpha status at v0.1.0. Features encrypted SQLite storage at rest, secrets engine with versioned key/value, transit engine for encryption-as-a-service, seal/unseal with Shamir secret sharing, and REST/gRPC APIs. KMS and PKI engines planned for future releases. Docker deployment with single command .

- **[Cosmian KMS](https://github.com/Cosmian/kms)**  
  Pure key management system in Rust following KMIP 1.4 standard. FIPS 140-3 compliant. Features complete key lifecycle (create, activate, revoke, destroy, rotate, compromise), native AES-256-GCM and ChaCha20, REST+KMIP dual interfaces, and external HSM support. Lightweight architecture focused solely on KMS functionality .

- **[RustyVault](https://github.com/rusty-vault/rusty-vault)**  
  Rust implementation with 100% API compatibility with HashiCorp Vault. Apache-2.0 licensed, addressing both license and China cryptography pain points. Built-in Tongsuo library for native SM2/SM3/SM4 envelope encryption. Memory-safe, high-concurrency performance, compatible with existing Vault Java SDKs. Supports Active-Active clustering, domestic HSM, and TEE trusted execution environments .

- **[Clef](https://github.com/clef-sh/clef)**  
  Tokenless secrets manager running entirely on Git and cloud KMS (MIT). Solves the "Secret Zero" problem without running a central server. Uses SOPS + Age encryption for local development, KMS envelope encryption for production delivery, and cloud IAM for authentication. The Clef Agent sidecar fetches secrets via localhost API. Trades infrastructure complexity for strict GitOps discipline .

- **[secrets (Go)](https://pkg.go.dev/github.com/allisson/secrets)**  
  Lightweight secrets manager in Go (MIT) inspired by HashiCorp Vault but intentionally simpler. Features envelope encryption, transit encryption, API auth with Argon2id, audit logs, and KMS integration (GCP, AWS, Azure, Vault). PostgreSQL backend. Not yet recommended for production at v0.x .

- **[SOPS (Mozilla)](https://github.com/mozilla/sops)**  
  Secrets encryption tool for configuration files (MPL-2.0). Structure-preserving encryption encrypts values while keeping file format intact. Integrates with AWS KMS, GCP KMS, Azure Key Vault, and PGP. Widely used for GitOps secret management .

- **[Sealed Secrets](https://github.com/bitnami-labs/sealed-secrets)**  
  Kubernetes secret encryption for GitOps (Apache-2.0). Encrypts secrets with a public key so they can be safely stored in public version control. Only the cluster's private key can decrypt. Features key rotation and offline recovery .

### Additional Strong Open-Source Options

- **[gopass](https://github.com/gopasspw/gopass)** — Terminal-based password manager using GPG and Git (MIT) for team secret sharing .
- **[aws-vault](https://github.com/99designs/aws-vault)** — Secure credential manager for AWS (MIT) using OS keystore and temporary sessions .
- **[git-secrets](https://github.com/awslabs/git-secrets)** — Prevents accidental credential commits via regex scanning (Apache-2.0) .
- **[Vault Secrets Operator](https://github.com/hashicorp/vault-secrets-operator)** — Kubernetes operator syncing Vault secrets to native K8s Secrets.
- **[External Secrets Operator](https://github.com/external-secrets/external-secrets)** — Kubernetes operator integrating external secret managers (Apache-2.0).
- Community **n8n** workflows for secret rotation automation and audit alerting.

**Frameworks for building custom systems**: Combine **OpenBao** or **Infisical** as the secrets management core with **SOPS** for GitOps-encrypted configuration, **Sealed Secrets** for Kubernetes-native secret delivery, **Cosmian KMS** for pure KMIP-compliant key management, and **PostgreSQL** for persistence — creating a fully self-hosted, enterprise-grade encryption key management platform.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Key management systems handling cryptographic material must comply with security standards (FIPS 140-2/3, SOC 2, PCI-DSS, etc.).
- Self-hosted open-source solutions require proper security hardening, HSM integration where required, and ongoing maintenance. Key custody is a security-critical operation demanding appropriate operational expertise.

---

**Made for security engineers, platform teams, compliance officers, and developers building transparent key management solutions.**  
Let's make Encryption Key Management more open, secure, and interoperable.
