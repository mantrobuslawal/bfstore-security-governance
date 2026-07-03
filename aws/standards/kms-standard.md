# Kms Standard

**Repository:** `bfstore-security-governance`  
**Status:** Draft v0.1  
**Last updated:** 2026-07-03

## Purpose

Define KMS key ownership, access and review patterns.

## Scope

Applies to all bfstore AWS accounts, repositories and platform workflows where relevant.

## bfstore position

bfstore uses a production-shaped AWS platform model: multi-account separation, federated workforce access, short-lived automation credentials, explicit workload identity, policy-as-code guardrails, central audit, and restore-tested backup strategies. The project deliberately self-manages selected platform components where that demonstrates operational competence, while documenting managed-service alternatives and trade-offs.

## Implementation guidance

- Separate key administration from key usage.
- Review key policies alongside IAM policies.
- Protect state, secrets, backups, logs and data stores.

## Required controls

- Exceptions documented.
- High-risk exceptions require ADR or review note.
- Controls should be testable and evidenced.

## Validation and evidence

- Quarterly review.
- Evidence stored under governance/evidence where applicable.



## References

- [IAM policies](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html)
- [AWS Organizations SCPs](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps.html)
- [CloudTrail](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-user-guide.html)
