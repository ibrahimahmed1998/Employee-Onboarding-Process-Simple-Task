Employee Onboarding Process Documentation
Summary
The design and implement an Employee Onboarding Process in Dynamics 365 CE that:
Routes onboarding requests to the correct HR Specialist based on department.
Uses a Retrieve Plugin to filter records by department.
Has JavaScript logic to auto-assign and lock the HR Specialist.
Enforces Business Rules, BPF stages, Field Security Profiles, and Workflows for routing and approvals.
Includes proper documentation, code, and a managed solution export.

 Conceptual Summary
The system is essentially a controlled onboarding workflow for new employees, where:
A Request Creator fills out an onboarding request.
The request is automatically assigned to the correct HR specialist using a mapping table.
The record progresses through HR Review → Manager Approval → Completion.
Each actor (HR, Manager) can only update their own approval field.
Visibility is governed by security and plugin-based filtering.
