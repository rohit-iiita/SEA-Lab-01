# Technical Root Causes: Healthcare.gov Launch Failure

## Overview

Technical root-cause analysis goes beyond identifying what broke. It
asks why the system was allowed to reach production with those problems
unresolved.

The supplied case material identifies several interconnected root
causes.

## 1. Poorly Managed Requirements

Requirements were not effectively managed, consistently approved, or
consistently linked to lower-level requirements.

### Why it mattered

Unclear or insufficiently controlled requirements created uncertainty
about system expectations and contributed to downstream development and
integration difficulties.

## 2. Development and Integration Difficulties

The system involved multiple IT systems and contractors.

Development and integration difficulties contributed to:

-   Incomplete functionality.
-   Software defects.
-   Problems that were not fully identified before launch.

## 3. Incomplete Functionality

Planned functionality was not completely implemented before the initial
launch.

### Root-cause significance

A system can pass individual checks while still being unready at the
system level if required functionality has not been fully integrated.

## 4. Unresolved Software Defects

Coding errors were identified but were not adequately corrected before
launch.

### Root-cause significance

Known defects represent a significant launch risk when their impact has
not been fully assessed and mitigated.

## 5. Insufficient System Testing

Healthcare.gov and its supporting systems were not fully tested before
launch.

The case material specifically identifies insufficient testing as a
major contributor.

### Root-cause significance

Without complete system-level testing, failures involving integration,
performance, and real-world behavior can remain hidden until production.

## 6. Inadequate Capacity Planning

The system was not adequately planned for expected workload and capacity
requirements.

### Root-cause significance

The production environment exposed the difference between expected
system behavior and real-world demand.

## 7. Weak Project Oversight

The supplied material identifies ineffective project oversight as a
contributing problem.

This allowed technical and process risks to persist instead of being
resolved or escalated effectively.

## Root-Cause Chain

The overall chain presented in the case material is:

**Poorly managed requirements**\
→ **Unclear / insufficiently controlled system expectations**\
→ **Development and integration difficulties**\
→ **Incomplete functionality + software defects**\
→ **Insufficient system testing**\
→ **Problems not fully identified/resolved before launch**\
→ **Inadequate capacity planning**\
→ **System unable to reliably handle real-world demand**\
→ **Healthcare.gov launch failure**

## Five Major Root-Cause Themes

1.  **Requirements management**
2.  **Development and integration**
3.  **Implementation quality**
4.  **Testing and verification**
5.  **Capacity and workload planning**

These technical causes interacted with organizational and management
problems described elsewhere in the lab, including weak risk management,
poor coordination, and unclear accountability.

## Key Lesson

The fundamental technical lesson is that a complex system must be
validated as a complete system---not merely as separate components.
Requirements must be controlled, functionality must be complete, known
defects must be addressed, integration must be tested, and expected
workload must be validated before production launch.
