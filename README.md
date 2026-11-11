# AWS IAM Privilege Escalation Lab
A hands-on AWS cloud security project exploring IAM privilege escalation, detection, and remediation.

## Project Overview

This lab demonstrates how misconfigured AWS IAM permissions can create privilege escalation risks and how security teams can identify and prevent them.

## Tools Used:

AWS Identity and Access Management (IAM), AWS IAM Policy Simulator, AWS CloudTrail, Amazon S3

## What I Did:

1. Setup: Created a limited IAM user with restricted permissions.
2. Attack Simulation: Used IAM Policy Simulator to demonstrate how iam:CreatePolicyVersion could allow privilege escalation if incorrectly granted.
3. Detection: Investigated IAM policy changes recorded in AWS CloudTrail.
4. Remediation: Verified least-privilege permissions and ensured the risky policy was not attached to any user.

## Screenshots

1. [Initial IAM permissions](screenshots/1-before-escalation.jpg)
2. [S3 access denied](screenshots/2-s3-access-denied.jpg)
3. [Policy Simulator - Denied](screenshots/3-policy-simulator-denied.jpg)
4. [Policy Simulator - Allowed](screenshots/4-policy-simulator-allowed.jpg)
5. [CloudTrail policy change](screenshots/5-cloudtrail-policy-change.jpg)
6. [Secure IAM policy](screenshots/6-secure-iam-policy.jpg)

Note: Privilege escalation was simulated using IAM Policy Simulator. No actual privilege escalation was performed.
