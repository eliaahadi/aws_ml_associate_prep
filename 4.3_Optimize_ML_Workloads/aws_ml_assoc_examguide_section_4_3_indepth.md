---
title: AWS Certified Machine Learning Engineer - Associate Exam Guide
---

# Section 4.3 --- Secure AWS Resources (In-Depth)

This section focuses on securing AWS ML infrastructure, data, and
pipelines. It includes IAM, encryption, network security, compliance,
and AWS tools for securing ML workflows.

## 1. IAM & Access Control

• IAM Roles → assign least-privilege roles to training, inference, and
pipelines.

• IAM Policies → control permissions for users, groups, and services.

• SageMaker Role Manager → simplifies IAM role creation for SageMaker
workflows.

• Best practice: follow principle of least privilege, audit regularly.

## 2. Data Security

• Encryption at Rest: SSE-S3, SSE-KMS, Client-side encryption (CSE).

• Encryption in Transit: TLS for API calls, VPC peering, PrivateLink.

• Key Management: AWS KMS for centralized encryption key management.

• Data Masking/Tokenization: protect sensitive fields (PII/PHI).

## 3. Network Security

• VPC Endpoints → secure communication between SageMaker and S3 without
leaving AWS network.

• Security Groups → control inbound/outbound traffic at instance level.

• NACLs (Network ACLs) → subnet-level traffic rules.

• PrivateLink → securely expose ML endpoints within private networks.

## 4. Compliance & Audit

• AWS Config → track compliance of ML resources against policies.

• AWS CloudTrail → log API calls and user actions for auditing.

• Amazon Macie → detect PII/PHI in data lakes and ML pipelines.

• GuardDuty → threat detection for anomalous activity in ML
environments.

• Organizations & SCPs → enforce guardrails across multiple AWS
accounts.

## 5. CI/CD Security Best Practices

• Store secrets in AWS Secrets Manager or SSM Parameter Store (never in
code).

• Use IAM roles instead of long-term access keys for pipelines.

• Implement least-privilege policies for
CodePipeline/CodeBuild/CodeDeploy.

• Sign and scan container images stored in Amazon ECR.

## 6. Best Practices

• Encrypt all data at rest and in transit by default.

• Apply least privilege to IAM roles and policies.

• Isolate ML systems inside VPCs with restricted security groups.

• Monitor and audit continuously with CloudTrail, Config, and GuardDuty.

• Regularly rotate IAM keys and secrets.

## ✅ Exam Tips

• IAM least-privilege principle is a recurring theme.

• SSE-KMS = exam's preferred encryption choice for sensitive data.

• VPC Endpoints = secure communication for SageMaker and S3.

• CloudTrail = auditing/logging, Config = compliance, Macie = PII
detection.

• Secrets Manager = manage API keys/secrets securely.
