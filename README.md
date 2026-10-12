# Awesome-Encryption-Key-Management

## Top Encryption Key Management Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Cryptographic Key Lifecycle, Secrets Management & Hardware Security*  

**Last updated: March 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Encryption Key Management**. These tools enable organizations to generate, store, rotate, and control access to cryptographic keys and secrets — securing data at rest, in transit, and across cloud environments while meeting compliance requirements.



**Examples** include Salesforce Key Management, HashiCorp Vault, AWS KMS, Azure Key Vault, Google Cloud KMS, Akeyless Vault, Fortanix DSM, Thales CipherTrust, Doppler, and CyberArk Conjur (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, hardware security module integration, and open key management — ideal for security engineers, platform teams, and organizations seeking transparent, vendor-independent encryption infrastructure.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)



## Sector Overview & Market Dynamics

The global Enterprise Key Management (EKM) and encryption software market is estimated at **$3.0B–$3.5B in 2025–2026**, growing at a CAGR of ~16–21% toward over $8B–$9B by the early 2030s driven by hybrid cloud sprawl, post-quantum cryptography (PQC) preparation, and regulatory compliance (GDPR, DORA, NIS2). The sector is **moderately fragmented yet tiered**: hyperscale cloud providers (Microsoft, Alphabet, AWS) dominate native cloud envelope encryption and infrastructure key custody, while specialized enterprise security providers (Thales, CyberArk, HashiCorp/IBM) and emerging SecretOps platforms (Infisical, Doppler, Akeyless) compete heavily for cross-cloud orchestration, secrets lifecycle, and zero-trust key management.

## SaaS/Hosted Platforms

| Product | Scale (Valuation / Revenue) | Starting Tier Pricing | Free Tier / Trial Limits | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[Alphabet (Google Cloud KMS)](https://cloud.google.com/security-key-management)** | ~$4.23T Market Cap (~$400B+ Ann. Revenue) | $0.06/key version/month + $0.03 per 10,000 key operations | **90-Day Free Trial** with $300 in cloud credits across GCP services | GCP native key management with Cloud EKM for external key control, Cloud HSM, and CMEK integration across GCP services. |
| **[Microsoft (Azure Key Vault)](https://azure.microsoft.com/en-us/products/key-vault/)** | ~$3.95T Market Cap (~$245B+ Ann. Revenue) | $0.03 per 10,000 operations for standard keys / secrets; Managed HSM starts at $3.20/hour | **Always Free Tier**: 20,000 free operations/month on standard tier (plus 30-day $200 Azure credit trial) | Azure native key, secret, and certificate management service featuring Managed HSM tier (FIPS 140-2 Level 3) and Entra RBAC. |
| **[Amazon (AWS KMS)](https://aws.amazon.com/kms/)** | ~$2.82T Market Cap (~$600B+ Ann. Revenue) | $1.00/month per customer-managed key (CMK) + $0.03 per 10,000 API requests beyond free tier | **Always Free Tier**: 20,000 requests/month across all regions (Free Tier does not cover $1/mo CMK fee) | Native AWS envelope encryption service integrated across virtually every AWS resource with multi-Region keys and CloudTrail audit logging. |
| **[Salesforce (Salesforce Shield)](https://help.salesforce.com/)** | ~$200B Market Cap (~$38B Ann. Revenue) | Platform Encryption priced at 20% of net annual Salesforce product spend (~$20,000+/year typical baseline) | **Free indefinitely on Developer Edition orgs** for testing; 30-day trial org available for enterprise evaluations | Shield Platform Encryption enabling customer-managed keys via BYOK or Cache-Only Key Service with HSM-backed key storage. |
| **[Thales (CipherTrust)](https://cpl.thalesgroup.com/)** | ~$52B Market Cap (€18B+ Ann. Revenue) | Enterprise subscription via private offer (~$1,000+/month base); Community Edition free software license | **CipherTrust Community Edition is Free Forever** (limited to 3 Kubernetes CTE worker nodes & 3 Data Protection Gateway clients; self-hosted infra costs apply) | Centralized enterprise key lifecycle platform offering database encryption, HSM integration, and multi-cloud key orchestration. |
| **[CyberArk (Conjur Cloud)](https://www.conjur.org/)** | ~$25B Acquisition by Palo Alto Networks (~$1B Ann. Revenue) | Billed per workload identity (~$40–$180/workload identity/year; minimum annual contract packages typically starting at $10k+/yr) | **No self-service cloud free tier**; custom sales-assisted guided PoC (typically 14–30 days); Conjur OSS is free forever self-hosted | Machine identity and secrets management platform with policy-as-code, dynamic secrets, and deep PAM suite integration. |
| **[HashiCorp / IBM (HCP Vault Dedicated)](https://www.hashicorp.com/cloud)** | $6.4B Acquisition by IBM (~$600M Ann. Revenue) | Development Tier starts at $0.616/cluster hour (~$450/month, single-node, max 25 clients); Production clusters from $1.58/hr | **$500 in free trial credits** valid for up to 6 months upon HCP account creation (restricted to single Vault cluster during trial) | Managed cloud Vault providing namespaces, automated replication, disaster recovery, transit encryption engine, and FIPS 140-2 support. |
| **[Akeyless Vault](https://www.akeyless.io/)** | ~$400M Valuation ($79M Raised) | Commercial Enterprise plans custom quoted based on client and dynamic secret volume | **Free Forever Tier**: Includes up to 5 clients, 500 static secrets, 5 dynamic secrets, 5 rotated secrets, and 5 RBAC roles/month | SaaS and hybrid secrets management platform utilizing distributed fragments technology (DFE) with zero-knowledge encryption and dynamic secrets. |
| **[Fortanix (Fortanix DSM)](https://www.fortanix.com/)** | ~$350M Valuation ($122M Raised) | Consumption-based subscription via cloud marketplace starting at ~$500–$1,000/month in app credits / private offers | **30-Day Free Trial** of Fortanix DSM SaaS Enterprise tier with full HSM-as-a-Service capabilities (no credit card required) | Data Security Manager with HSM-as-a-Service, FIPS 140-2 Level 3 validated HSMs, confidential computing, and multi-cloud key orchestration. |
| **[Doppler](https://www.doppler.com/)** | ~$75M Valuation ($44M Raised) | Team Tier starts at $18/month (includes first 3 users; additional users at $6/user/month); Developer Tier free | **Free Forever Developer Plan**: Free for up to 3 users with universal secret management, environments, and CLI workflows | Developer-first SecretOps platform with CLI-driven workflows, multi-environment syncing, and secret rotation integrations. |





## Open-Source GitHub Projects

Curated list of open-source encryption key managers, secrets management systems, and cryptographic tooling, sorted in descending order by GitHub stars.

- **[HashiCorp Vault](https://github.com/hashicorp/vault)** [![Stars](https://img.shields.io/github/stars/hashicorp/vault?style=social&color=white)](https://github.com/hashicorp/vault/stargazers)  
  The industry benchmark for open-source secrets management (BSL 1.1). Features static and dynamic secrets, transit engine for encryption-as-a-service, PKI certificate issuance, tokenization transform engine, and over 15 pluggable authentication backends.

- **[Infisical](https://github.com/Infisical/infisical)** [![Stars](https://img.shields.io/github/stars/Infisical/infisical?style=social&color=white)](https://github.com/Infisical/infisical/stargazers)  
  Open-source platform for securing secrets, certificates, and privileged access management (MIT/Enterprise). Features end-to-end encrypted secrets vaulting, internal KMS for customer keys, native PKI/CA, SSH certificate authority, and native Kubernetes syncing.

- **[age](https://github.com/FiloSottile/age)** [![Stars](https://img.shields.io/github/stars/FiloSottile/age?style=social&color=white)](https://github.com/FiloSottile/age/stargazers)  
  A simple, modern, and secure file encryption tool and Go library featuring small explicit keys, no configuration requirements, UNIX-pipeline composability, and plugin support for hardware tokens (YubiKey / PIV).

- **[SOPS](https://github.com/getsops/sops)** [![Stars](https://img.shields.io/github/stars/getsops/sops?style=social&color=white)](https://github.com/getsops/sops/stargazers)  
  Structure-preserving secrets editor and encryption tool (MPL 2.0). Encrypts YAML, JSON, ENV, and INI values while leaving data keys intact. Deeply integrates with AWS KMS, GCP KMS, Azure Key Vault, HashiCorp Vault, and age.

- **[git-secrets](https://github.com/awslabs/git-secrets)** [![Stars](https://img.shields.io/github/stars/awslabs/git-secrets?style=social&color=white)](https://github.com/awslabs/git-secrets/stargazers)  
  Prevents developers and CI/CD pipelines from committing private keys, secrets, and AWS credentials into Git repositories via configurable commit-hook regex scanning (Apache 2.0).

- **[Sealed Secrets](https://github.com/bitnami-labs/sealed-secrets)** [![Stars](https://img.shields.io/github/stars/bitnami-labs/sealed-secrets?style=social&color=white)](https://github.com/bitnami-labs/sealed-secrets/stargazers)  
  Kubernetes controller and tool for one-way encrypted Secrets (Apache 2.0). Encrypts secrets using asymmetric public keys for safe storage in public Git repos, with private decryption keys restricted to the target cluster.

- **[aws-vault](https://github.com/99designs/aws-vault)** [![Stars](https://img.shields.io/github/stars/99designs/aws-vault?style=social&color=white)](https://github.com/99designs/aws-vault/stargazers)  
  CLI tool for securely storing and accessing AWS credentials in developer environments (MIT). Encrypts API keys in the operating system's native keystore (macOS Keychain, Secret Service, Windows Credential Manager) and issues temporary STS credentials.

- **[step-ca (smallstep)](https://github.com/smallstep/certificates)** [![Stars](https://img.shields.io/github/stars/smallstep/certificates?style=social&color=white)](https://github.com/smallstep/certificates/stargazers)  
  Private certificate authority (X.509 and SSH) and ACME server (Apache 2.0). Provides automated key generation, certificate issuance, TPM/HSM-backed cryptographic key protection, and mutual TLS orchestration.

- **[OpenBao](https://github.com/openbao/openbao)** [![Stars](https://img.shields.io/github/stars/openbao/openbao?style=social&color=white)](https://github.com/openbao/openbao/stargazers)  
  Community-governed fork of HashiCorp Vault hosted by the Linux Foundation under the MPL 2.0 license. Provides drop-in API compatibility for managing secrets, issuing PKI certificates, and providing transit encryption without commercial licensing friction.

- **[gopass](https://github.com/gopasspw/gopass)** [![Stars](https://img.shields.io/github/stars/gopasspw/gopass?style=social&color=white)](https://github.com/gopasspw/gopass/stargazers)  
  Standard UNIX-style password and cryptographic secret manager for teams (MIT). Built with GPG and Git, featuring multi-store synchronization, secret sharing hierarchies, and audit capabilities.

- **[External Secrets Operator](https://github.com/external-secrets/external-secrets)** [![Stars](https://img.shields.io/github/stars/external-secrets/external-secrets?style=social&color=white)](https://github.com/external-secrets/external-secrets/stargazers)  
  Kubernetes operator that integrates external secret management APIs (AWS Secrets Manager/KMS, HashiCorp Vault, Azure Key Vault, Google Secret Manager, Akeyless) directly into native Kubernetes Secret manifests (Apache 2.0).

- **[OpenSC](https://github.com/OpenSC/OpenSC)** [![Stars](https://img.shields.io/github/stars/OpenSC/OpenSC)](https://github.com/OpenSC/OpenSC/stargazers)  
  Open-source smart card middleware and cryptographic tools (LGPL 2.1). Implements PKCS#11 API and cryptographic token interfaces for hardware security modules (HSMs), smart cards, and hardware crypto devices.

- **[Keywhiz](https://github.com/square/keywhiz)** [![Stars](https://img.shields.io/github/stars/square/keywhiz?style=social&color=white)](https://github.com/square/keywhiz/stargazers)  
  Square's system for distributing and managing sensitive cryptographic keys and secrets across distributed application fleets (Apache 2.0). Features mutual TLS, encrypted persistence, and automated access policies.

- **[Confidant](https://github.com/lyft/confidant)** [![Stars](https://img.shields.io/github/stars/lyft/confidant?style=social&color=white)](https://github.com/lyft/confidant/stargazers)  
  Lyft's open-source secrets keeper (Apache 2.0). Uses AWS KMS for client-side authentication and encryption of secrets stored in DynamoDB, eliminating the operational overhead of central master key unsealing.

- **[Athenz](https://github.com/yahoo/athenz)** [![Stars](https://img.shields.io/github/stars/yahoo/athenz?style=social&color=white)](https://github.com/yahoo/athenz/stargazers)  
  Open-source platform by Yahoo/OATH for X.509 certificate-based service authentication and fine-grained role-based authorization across dynamic cloud infrastructure (Apache 2.0).

- **[Conjur OSS](https://github.com/cyberark/conjur)** [![Stars](https://img.shields.io/github/stars/cyberark/conjur?style=social&color=white)](https://github.com/cyberark/conjur/stargazers)  
  CyberArk's open-source container-native secrets management engine (Apache 2.0). Implements policy-as-code for microservice machine identities, secret retrieval, and role-based access control.

- **[tpm2-tools](https://github.com/tpm2-software/tpm2-tools)** [![Stars](https://img.shields.io/github/stars/tpm2-software/tpm2-tools?style=social&color=white)](https://github.com/tpm2-software/tpm2-tools/stargazers)  
  Core user-space toolset for interacting with Trusted Platform Module (TPM 2.0) chips (BSD 3-Clause). Enables hardware-backed key creation, sealing, quote attestation, and cryptographic operations.

- **[go-tpm](https://github.com/google/go-tpm)** [![Stars](https://img.shields.io/github/stars/google/go-tpm?style=social&color=white)](https://github.com/google/go-tpm/stargazers)  
  Google's Go library providing low-level and high-level interfaces to interact directly with TPM 1.2 and TPM 2.0 devices for hardware-rooted key lifecycle management and measurements (BSD 3-Clause).

- **[Vault Secrets Operator](https://github.com/hashicorp/vault-secrets-operator)** [![Stars](https://img.shields.io/github/stars/hashicorp/vault-secrets-operator?style=social&color=white)](https://github.com/hashicorp/vault-secrets-operator/stargazers)  
  Official Kubernetes operator developed by HashiCorp to synchronize secrets and cryptographic keys stored in Vault directly into Kubernetes cluster secrets (MPL 2.0).

- **[RustyVault](https://github.com/Tongsuo-Project/RustyVault)** [![Stars](https://img.shields.io/github/stars/Tongsuo-Project/RustyVault?style=social&color=white)](https://github.com/Tongsuo-Project/RustyVault/stargazers)  
  Rust implementation featuring API compatibility with HashiCorp Vault (Apache 2.0). Built on the Tongsuo cryptographic library with native SM2/SM3/SM4 envelope encryption, memory safety, and TEE/HSM backend support.

- **[Cosmian KMS](https://github.com/Cosmian/kms)** [![Stars](https://img.shields.io/github/stars/Cosmian/kms?style=social&color=white)](https://github.com/Cosmian/kms/stargazers)  
  Lightweight Key Management System written in Rust implementing the OASIS KMIP 1.4/2.x standards. Features AES-256-GCM, ChaCha20, complete key lifecycles, and external PKCS#11 HSM integration.

- **[Clef](https://github.com/clef-sh/clef)** [![Stars](https://img.shields.io/github/stars/clef-sh/clef?style=social&color=white)](https://github.com/clef-sh/clef/stargazers)  
  Tokenless secrets manager running on Git and cloud KMS (MIT). Eliminates the "Secret Zero" dilemma using SOPS + age for local developer encryption and cloud IAM envelope encryption for production delivery.

- **[secrets](https://github.com/allisson/secrets)** [![Stars](https://img.shields.io/github/stars/allisson/secrets?style=social&color=white)](https://github.com/allisson/secrets/stargazers)  
  Minimalist secrets manager in Go (MIT). Features envelope encryption, transit encryption, Argon2id API authentication, and KMS provider integrations with PostgreSQL storage.

- **[Egide](https://github.com/nubster-opensources/egide)** [![Stars](https://img.shields.io/github/stars/nubster-opensources/egide?style=social&color=white)](https://github.com/nubster-opensources/egide/stargazers)  
  Self-hosted secrets manager in Rust. Features encrypted SQLite storage at rest, versioned key/value engines, transit encryption-as-a-service, and Shamir's Secret Sharing unseal mechanics.



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
