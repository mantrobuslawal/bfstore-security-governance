# Root Account Controls

**Repository:** `bfstore-security-governance`  
**Status:** Draft v0.1  
**Last updated:** 2026-07-03

## Purpose

Ensure root users are protected and never used for day-to-day work.

## Scope

Control definition, implementation notes and evidence expectations.

## bfstore position

bfstore uses a production-shaped AWS platform model: multi-account separation, federated workforce access, short-lived automation credentials, explicit workload identity, policy-as-code guardrails, central audit, and restore-tested backup strategies. The project deliberately self-manages selected platform components where that demonstrates operational competence, while documenting managed-service alternatives and trade-offs.

## Implementation guidance

- Root MFA enabled.
- Root access keys absent.
- Root credentials stored securely.
- Root usage alerts enabled where practical.

## Required controls

- Root MFA enabled.
- Root access keys absent.
- Root credentials stored securely.
- Root usage alerts enabled where practical.

## Validation and evidence

- Control implementation reviewed.
- Evidence stored in relevant folder.
- Exceptions documented.



## References

- [IAM Access Analyzer](https://docs.aws.amazon.com/IAM/latest/UserGuide/what-is-access-analyzer.html)
- [CloudTrail](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-user-guide.html)
- [AWS Backup service roles](https://docs.aws.amazon.com/aws-backup/latest/devguide/iam-service-roles.html)
- [KMS key policies](https://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html)
