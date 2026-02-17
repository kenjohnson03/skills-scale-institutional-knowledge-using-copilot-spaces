# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted by **Release Manager**
- Rollback / mitigation plan documented
- Smoke tests prepared
- **UX Designer**: Design QA completed for UI changes
- **Customer Support Liaison**: Support documentation and FAQs updated

## Deployment Checklist
- [ ] Deployment window scheduled (if needed) — coordinated by **Release Manager**
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] **UX Designer**: Verify UI changes in staging environment
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] **Release Manager**: Announce release to stakeholders and support
- [ ] **Customer Support Liaison**: Brief support team on changes and new features

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - **Release Manager**: Coordinate rollback to last known-good release if necessary
  - Triage root cause and capture action items
  - **Customer Support Liaison**: Communicate status to affected customers

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
