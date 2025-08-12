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
