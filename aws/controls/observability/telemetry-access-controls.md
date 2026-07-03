# Telemetry Access Controls

**Repository:** `bfstore-security-governance`  
**Status:** Draft v0.1  
**Last updated:** 2026-07-03

## Purpose

Control access to logs, metrics, traces and dashboards.

## Scope

Control definition, implementation notes and evidence expectations.

## bfstore position

bfstore uses a production-shaped AWS platform model: multi-account separation, federated workforce access, short-lived automation credentials, explicit workload identity, policy-as-code guardrails, central audit, and restore-tested backup strategies. The project deliberately self-manages selected platform components where that demonstrates operational competence, while documenting managed-service alternatives and trade-offs.

## Implementation guidance

- Application logs may be less restricted than security/audit logs.
- Central observability outside prod.
- Sensitive data redaction reviewed.

## Required controls

- Application logs may be less restricted than security/audit logs.
- Central observability outside prod.
- Sensitive data redaction reviewed.

## Validation and evidence

- Control implementation reviewed.
- Evidence stored in relevant folder.
- Exceptions documented.



## References

- [IAM Access Analyzer](https://docs.aws.amazon.com/IAM/latest/UserGuide/what-is-access-analyzer.html)
- [CloudTrail](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-user-guide.html)
- [AWS Backup service roles](https://docs.aws.amazon.com/aws-backup/latest/devguide/iam-service-roles.html)
- [KMS key policies](https://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html)
