# cst8919-a2

In the following report, I will organize the report based on each service.

# 1. Azure Active Directory (SSO, IAM)

Overview: Azure Active Directory (now Microsoft Entra ID) is a cloud IAM service. It provides SSO, MFA, and conditional access. It protects access to cloud and on-premises resources.

| Category | Azure Active Directory | AWS IAM & AWS SSO | Google Cloud Identity |
| :--- | :--- | :--- | :--- |
| Core Features | Central identity for users. SSO for SaaS apps. Conditional access policies. | AWS IAM for fine-grained permissions. AWS SSO (now IAM Identity Center) for centralized access. | Central identity provider. Managed users and groups. SSO for Google Workspace and third-party apps. |
| Security & Compliance | Supports MFA, conditional access, and PIM. Compliant with various standards like SOC 2 and ISO 27001. | IAM provides roles for least-privilege access. IAM Access Analyzer finds overly permissive policies. | Strong security with SSO and MFA. Integrates with Security Center. Compliant with many frameworks. |
| Pricing Model | Free tier for basic features. Premium plans have a per-user, per-month charge for advanced features like PIM. | AWS IAM is free. AWS SSO is also free. Costs are for underlying services. | Free tier for core services. Paid plans for advanced features like security reports. |
| Integration for DevSecOps | Integrates with Azure DevOps and GitHub. Used for identity-based access control in CI/CD. | IAM roles are fundamental for CI/CD automation. Can use SAML federation with CI/CD tools. | Integrates with GCP services like Cloud Build. Cloud IAM roles grant permissions to CI/CD services. |

# 2. Azure Monitor & Log Analytics

Overview: Azure Monitor is a comprehensive monitoring solution. Log Analytics is a feature of Azure Monitor. It provides a query language and workspace for analyzing logs.

| Category | Azure Monitor & Log Analytics | AWS CloudWatch & CloudWatch Logs | Google Cloud Observability |
| :--- | :--- | :--- | :--- |
| Core Features | Collects metrics and logs. Log Analytics uses KQL for querying. Application Insights for app performance. | CloudWatch for metrics and dashboards. CloudWatch Logs for log aggregation. Log Insights for querying logs. | Cloud Logging for log collection. Cloud Monitoring for metrics and dashboards. Uses a SQL-like query language. |
| Security & Compliance | Centralized logging for security events. Provides audit trails. Helps meet compliance with historical data. | Centralizes logs for services like CloudTrail. CloudWatch Alarms can monitor for compliance events. | Centralized logs for auditing. Integrates with Security Command Center. |
| Pricing Model | Charged based on data ingestion and retention. Per-GB pricing model for Log Analytics. | Free tier for basic metrics. Custom metrics and log data are charged per GB. Log Insights is priced per GB of data scanned. | Pricing based on data ingestion. Log data over a certain size is charged per GB. Free tier includes a generous amount of data. |
| Integration for DevSecOps | Essential for monitoring CI/CD health. Log Analytics is used to troubleshoot deployment failures. | CloudWatch can trigger alerts on CI/CD metrics. Provides feedback on pipeline health. | Integrates with Cloud Build and other services. Provides real-time logs for CI/CD processes. |


# 3. Azure Policy

Overview: Azure Policy helps enforce organizational standards. It defines rules for resource creation and updates. It ensures new resources are compliant with security requirements.

| Category | Azure Policy | AWS Config | Google Cloud Policy Intelligence |
| :--- | :--- | :--- | :--- |
| Core Features | Audits and enforces resource configurations. Supports built-in and custom policies. Provides compliance dashboards. | Continuously records configurations and changes. Evaluates compliance against rules. | Recommends policies based on usage. Manages IAM policies. Not a direct enforcement tool. |
| Security & Compliance | Enforces security best practices. Integrates with Defender for Cloud for compliance reports. | Audits resources against compliance benchmarks (CIS, PCI). Provides a timeline of configuration changes. | Helps analyze and manage IAM policies. Policy Analyzer checks if a principal has permissions. |
| Pricing Model | No cost for policy definitions. Cost is from underlying services and remediation. | Priced on number of configuration items and rules. Free tier for limited evaluations. | Not a separate service with its own pricing. Part of Cloud IAM, which is a free service. |
| Integration for DevSecOps | Can be used in CI/CD to validate templates. Ensures compliance by design. | AWS Config validates resources deployed by a CI/CD pipeline. Can trigger remediation via Lambda. | Helps developers understand the security impact of code. Provides insights into permissions and policies. |



# 4. Microsoft Defender for Cloud

Overview: Defender for Cloud is a CSPM and CWP solution. It provides unified security management and threat protection. It supports hybrid and multi-cloud environments.

| Category | Defender for Cloud | AWS Security Hub | Google Security Command Center |
| :--- | :--- | :--- | :--- |
| Core Features | Central security score. Threat protection for servers, containers, databases. Multi-cloud support. | Central dashboard for security alerts. Automated compliance checks. Consolidates findings from many AWS services. | Centralized platform for security and risk. Offers asset discovery and vulnerability scanning. |
| Security & Compliance | Regulatory compliance dashboard. Assesses compliance against HIPAA and PCI DSS. | Consolidates compliance findings from AWS services. Checks against industry standards. | Provides a "compliance" view. Helps track posture against benchmarks like CIS. |
| Pricing Model | CSPM features are free. Advanced CWP plans are charged per-resource (e.g., per-server). | Based on number of security checks and findings ingested. Free tier for the first 10,000 findings. | Premium tier is based on the number of protected resources. Standard tier is free. |
| Integration for DevSecOps | Scans container images for vulnerabilities in CI/CD. Provides recommendations to developers. | Ingests findings from CI/CD tools. Developers can see security issues early. | Scans for misconfigurations. Findings can be routed to developers. |


# 5. Azure Sentinel (SIEM/SOAR)

Overview: Azure Sentinel (now Microsoft Sentinel) is a cloud-native SIEM and SOAR solution. It provides a single pane of glass for security analytics. It offers threat intelligence across the enterprise.

| Category | Azure Sentinel | AWS GuardDuty & Security Hub | Google Security Command Center |
| :--- | :--- | :--- | :--- |
| Core Features | SIEM/SOAR capabilities. Ingests data from many sources. Playbooks for automated responses. | GuardDuty is a threat detection service. Security Hub aggregates findings for a SIEM. | A central hub for security findings. Integrates with Chronicle Security Operations for SIEM/SOAR. |
| Security & Compliance | Provides advanced threat detection. Centralizes security data for auditing. Helps meet compliance requirements. | GuardDuty uses ML to detect threats. Security Hub centralizes compliance findings from various services. | Offers a high-level view of security posture. Helps detect threats and vulnerabilities. |
| Pricing Model | Priced based on data ingestion (per GB). There are tiers based on commitment. | GuardDuty pricing is based on data analyzed. Security Hub is priced per check and per finding. | The Standard tier is free. The Premium tier has a fee based on protected resources. |
| Integration for DevSecOps | Can ingest logs from CI/CD pipelines. Detects suspicious activity like unauthorized deployments. | Security Hub findings provide security feedback to CI/CD. GuardDuty monitors access keys used in pipelines. | Monitors CI/CD pipelines for threats. Findings can trigger automated remediation via Cloud Functions. |

