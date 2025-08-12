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
