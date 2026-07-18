# Multi-Cloud Identity Engineering: Passwordless Workload Federation Framework

## The Big Picture (Plain Language Summary)
In the world of Physical AI—which includes autonomous vehicles, robotics, and defense hardware—computers are constantly talking to other computers. To train an autonomous car or run a simulation, automated software "bots" must pull highly sensitive code and data out of secure digital vaults. 

Traditionally, engineers grant these bots access by giving them static passwords or secrets. The massive flaw? If a human accidentally leaks that password, a malicious actor can steal proprietary AI models or corrupt the real-world machinery.

This repository demonstrates a mini-project that completely solves this problem. It serves as a live execution of the **AI and Cloud Pipeline Hardening Framework**, a structured architectural process developed by Steven Tuschman. Instead of using vulnerable passwords, this framework establishes a "passwordless digital handshake" (Workload Identity Federation) between the automated bots and the cloud perimeter. The bot presents a short-lived, cryptographically signed digital token that automatically expires after 60 minutes, making long-term identity theft virtually impossible

---

## My Methodology: The Process & The Ledger
I do not configure cloud security in a freeform or casual manner. This project is a direct demonstration of how my framework applies a strict, predictable engineering blueprint to any target industry. 

The mandatory, standard output of this process is the **Identity Architecture Ledger (IAL)**. The ledger is a master engineering record that maps every moving part of the identity plane down to hard boolean (True/False) verification gates. By utilizing this ledger system, I ensure that any machine identity I configure is 100% auditable, fully compliant with Zero Trust parameters, and completely reproducible across different multi-cloud environments.

---

## Real-World Industry Application
While the underlying passwordless handshake uses a universal framework, this specific lab is tailored to mirror the operational realities of the **Physical AI and Autonomous Systems** sector. The technical controls are mapped to defend real-world machine topologies:

1. **Simulation Ingestion Agents:** Securing the automated software runners that push massive streams of synthetic sensor and camera telemetry data into the cloud.
2. **Autonomous AI Workloads:** Restricting non-human training agents to strict, least-privilege boundaries so they can only fetch the explicit signing keys they need to function.

---

## Architectural Blueprint & System Ledger (IAL Snapshot)

This lab run isolates, provisions, and completely validates a hardened cross-platform handshake using raw configuration standards necessary to bypass legacy, broken user-interface wizards.

### 1. Directory Boundary & Target Coordinates
*   **Identity System Boundary:** Microsoft Entra ID Tenant
*   **Secure Container (Digital Vault):** Azure Key Vault (`kv-autonomous-secrets-prod`)
*   **Protected Asset (The Target):** Simulation Model Signing Keys (`SIM_MODEL_SIGNING_KEY`)

### 2. The Passwordless Handshake Rule
*   **External Authority (The Passport Issuer):** GitHub Token Service
*   **Modern Validation Protocol:** The system is explicitly configured using a custom **Other Issuer** rule. This matches the bot's identity directly to an **Immutable Subject Claim Profile** containing the source repository's unique, unchangeable database tracking numbers. If an attacker tries to maliciously copy or rename the repository, the identity registry instantly drops the connection.

### 3. Framework Verification Gates (Hard Booleans)
The absolute structural integrity of this lab is verified within the ledger by four explicit check gates:
*   `YAML Parse Success`: **Core Execution Phase** -> The automation scripts are perfectly formatted and isolated.
*   `OIDC Handshake Success`: **Authentication Phase** -> The identity plane accepted the digital passport and granted entry.
*   `Data Row Extract Success`: **Authorization Phase** -> The machine bot successfully reached into the vault without a password.
*   `Payload Identity Matches`: **Verification Phase** -> Automated telemetry logs confirm the retrieved secret is verified and intact.


# ENTERPRISE ENGINEERING SPECIFICATION: IDENTITY ARCHITECTURE LEDGER (IAL)

### Project Metadata Baseline
*   **Deployment System Target:** GitHub Runner Pipeline
*   **Target Cloud Provider:** Microsoft Azure
*   **Execution Date:** 2026-07-18
*   **Compliance Status:** Pass
*   **AI Ingestion Agent Status:** Enabled

---

## SECTION 1: CORE CLOUD BOUNDARY IDENTIFICATION

### 1.1 Structural Boundary Discovery Matrix
This matrix anchors the globally unique root coordinates of the identity directory and the targeted asset deployment environment.
*   **Resource A (Source Identity Center) - Tenant ID:** `9439dd25-f3b5-4829-a76f-5ede8cd54c3c`
*   **Resource B (Target Asset Environment) - Subscription ID:** `d5ffd8a5-d994-4eb5-b87c-4442054d233e`

### 1.2 Asset Configuration Profile
Track the live state of the physical infrastructure assets deployed inside the target resource boundary.
*   **Target Cloud Asset Type:** Azure Key Vault
*   **Provisioned Resource Name:** `kv-compcode1-ai-vault`
*   **Resource Group Perimeter:** [Not Specified / Inherited from Vault Scope]

### 1.3 Automated Telemetry Sourcing Method
*   [X] **Manual Lookup:** Extracted from portal browser surfaces.
*   [ ] **AI Agent Programmatic Discovery:** Automated JSON variable extraction via CLI/PowerShell script telemetry.

### 1.4 Operational Identity Validation Gate
Before moving past Phase 1, the following logical condition must be manually audited or AI-verified.

> **[ HARD BOOLEAN VALIDATION ]** Are both the target subscription asset and the identity directory actively nested under the identical root tenant domain structure?
*   [X] **SUCCESS:** Workspace paths cryptographically align. AI agent records identifiers.
*   [ ] **FAILURE / INTERRUPTED:** Mismatched tenant directory context detected. Cross-cloud routing will fail validation before token issuance.

---

## SECTION 2: NON-HUMAN IDENTITY PROVISIONING

### 2.1 Identity Object Profile
Document the primary administrative naming convention and unique identifier generated for the machine account.
*   **Configured Application Name:** `identity-ai-bot`
*   **Application (Client) ID:** `22df9133-520e-4fd6-b456-e564190116fc`

### 2.2 Architectural Tenancy and Redirection Boundaries
Enforce the structural constraints chosen during the initialization of the application object.

**Supported Account Type Selection:**
*   [X] **Potential A: Single-Tenant** (Accounts in this organizational directory only - standard for internal enterprise/AI workloads)
*   [ ] **Potential B: Multi-Tenant** (Accounts in any organizational directory - required for external B2B SaaS applications)
*   [ ] **Potential C: Multi-Tenant and Personal Microsoft Accounts** (Enterprise software with integrated consumer account access)
*   [ ] **Potential D: Personal Microsoft Accounts Only** (Isolates identity entirely within the consumer-grade ecosystem)

**Redirect URI (Reply URL) Configuration:**
*   [X] **Left Entirely Blank** (Optimized for headless background runners and automated AI workloads)
*   [ ] **Populated** (Interactive web application human-login redirection routing)

### 2.3 Operational Identity Validation Gate
Before moving past Phase 2, the following logical condition must be audited and affirmed.

> **[ HARD BOOLEAN VALIDATION ]** Has the directory portal successfully initialized both the Application Object blueprint and the local enterprise Service Principal card?
*   [X] **SUCCESS:** Both structural objects exist in the tenant; Application ID is recorded into the ledger by the AI runtime context.
*   [ ] **FAILURE / INTERRUPTED:** Registration incomplete or app suspended. External runners cannot reference the identity.

---

## SECTION 3: PASSWORDLESS CRYPTOGRAPHIC FEDERATION

### 3.1 Federated Trust Parameters
Document the precise OpenID Connect (OIDC) metadata properties configured to anchor the cross-platform trust root.
*   **Federated Credential Name:** `universal-pipeline-handshake`
*   **Issuer URL:** `https://token.actions.githubusercontent.com`
*   **Audience Mapping:** `api://AzureADTokenExchange`

### 3.2 Selected Architectural Scenario Boundary
*   [ ] **GitHub Actions:** CI/CD automation pipeline tracking.
*   [ ] **Kubernetes Workloads:** Maps trust to container cluster OpenID Connect Issuer URL.
*   [ ] **Managed Identity:** Cross-app localized trust anchor between distinct application objects.
*   [X] **Other Issuer:** Custom external vendor platforms utilizing raw string entries.

### 3.3 Granular Subject Claim and Entity Mapping
Record the explicit, case-sensitive string used to isolate inbound authentication directly to your approved code or runtime perimeter.
*   **Target Repository Owner / Org:** `Compcode1`
*   **Target Repository Name:** `workload-federation-physical-ai`

**Target Entity Type Deployment Gate:**
*   [ ] Environment
*   [X] Branch
*   [ ] Pull Request
*   [ ] Tag

*   **Target Execution Path Name (Branch/Env/Tag Name):** `main`
*   **Final Computed Subject String (sub):** `repo:[Org]@[OrgID]/[Repo]@[RepoID]:ref:[Path]`
*   **Actual Form:** `repo:Compcode1@171821203/workload-federation-physical-ai@1304885124:ref:refs/heads/main`

### 3.4 Security Invariant Checklist
Verify compliance against strict zero-trust identity isolation boundaries.
*   [ YES ] Is the final Subject identifier completely explicit and free of broad production wildcards (*)?
*   [ YES ] Has the exact string casing been verified against the external repository path to prevent silent character-match failure states?

### 3.5 Operational Identity Validation Gate
Before moving past Phase 3, the following logical condition must be audited and affirmed.

> **[ HARD BOOLEAN VALIDATION ]** Has the cryptographic policy been successfully written into the Application Object's federated identity collection and locked?
*   [X] **SUCCESS:** Trust policy is active; identity token endpoint is listening for matching external claims. AI logs verified configurations.
*   [ ] **FAILURE / INTERRUPTED:** Policy misconfiguration or invalid issuer URL string. Inbound handshakes will trigger immediate authentication drops.

---

## SECTION 4: DATA-PLANE ACCESS ENFORCEMENT & PIPELINE EXECUTION

### 4.1 Role-Based Access Control (RBAC) Entitlements
Document the precise data-plane authorization scope assigned to the local Service Principal inside the resource target perimeter.
*   **Assigned Data-Plane Role:** Key Vault Secrets User / Key Vault Data Plane Access Policy
*   **Target Resource Attachment Scope:** `kv-compcode1-ai-vault`

### 4.2 Token State & Lifecycle Controls
Map out the hard cryptographic token thresholds governing the lifecycle of the active automation run.
*   **Access Token (AT) Expiration Ceiling:** 60 Minutes (Absolute value active for data-plane read/write actions)
*   **Refresh Token (RT) Availability:** 0 Minutes (Blocked natively - long running scripts must execute a new OpenID Connect handshake)

### 4.3 Log-Leak Mitigation & Script Hardening
Identify and apply explicit text-masking boundaries to intercept raw string outputs before they hit public build screens.

**Telemetry Masking Rule Status:**
*   [ YES ] Repository environment variables are actively hidden (***) by the runner framework.
*   [ YES ] Script-level output suppression commands and runtime masking directives are explicitly coded to intercept and redact dynamic data-plane variables in memory.

### 4.4 Operational Identity Validation Gate
Before finalizing the ledger, the following logical condition must be audited and affirmed within the environment telemetry.

> **[ HARD BOOLEAN VALIDATION ]** Has the machine runner bypassed broad infrastructure control roles and successfully authenticated directly against a data-plane role?
*   [X] **SUCCESS:** Pipeline logs show clean authorization and zero 403 Forbidden drop faults during asset reading. AI records a success state.
*   [ ] **FAILURE / INTERRUPTED:** Authentication returns a success state, but subsequent asset data access drops with a standard 403 authorization error.
