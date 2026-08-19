# Requirements, Design & Implementation Issues: Healthcare.gov

## Overview

The Healthcare.gov failure involved problems at multiple stages of
software development: requirements, design, and implementation.

The important distinction is between:

-   **Requirements:** deciding what the system should do.
-   **Design:** planning how the system should work and how it should
    meet workload and technical needs.
-   **Implementation:** developing the actual software and
    functionality.

## 1. Requirements Issues

The requirements were not effectively managed.

The supplied SDLC analysis identifies that requirements were:

-   Not effectively managed.
-   Not consistently approved.
-   Not consistently linked to lower-level requirements.

This represents a **Requirements Failure (C1)**.

### Consequence

Poorly controlled requirements contributed to unclear or insufficiently
controlled system expectations. This then contributed to development and
integration difficulties.

## 2. Design Issues

The system was not adequately planned for expected workload and capacity
requirements.

This issue originated in the **Requirements / Design** phase and was
detected in **Production**.

### Consequence

The lack of adequate capacity planning meant that the system could not
reliably handle real-world demand after launch.

## 3. Implementation Issues

Planned functionality was not completely implemented before the initial
launch.

The supplied SDLC mapping places this problem in **Requirements /
Implementation**, with detection occurring during **Testing /
Production**.

Software coding errors were also identified but were not adequately
corrected before launch.

This represents an **Implementation Failure (C4)**.

## 4. Relationship Between the Problems

The problems formed a chain:

**Poor requirements management**\
→ unclear system expectations\
→ development and integration difficulties\
→ incomplete functionality and software defects\
→ insufficient testing\
→ unresolved problems reaching production.

Capacity planning was another important branch:

**Requirements / design problems**\
→ inadequate capacity planning\
→ inability to reliably handle expected demand\
→ production performance problems.

## Summary

  -----------------------------------------------------------------------
  Area                    Problem                 Consequence
  ----------------------- ----------------------- -----------------------
  Requirements            Requirements were not   Unclear or
                          effectively managed or  insufficiently
                          consistently            controlled expectations
                          approved/linked         

  Design                  Workload and capacity   System could not
                          requirements were not   reliably handle
                          adequately planned      real-world demand

  Implementation          Planned functionality   System launched without
                          was incomplete          all intended
                                                  functionality

  Implementation          Coding errors were not  Defects remained before
                          adequately corrected    launch

  Integration             Development and         Contributed to
                          integration             incomplete
                          difficulties occurred   functionality and
                                                  defects
  -----------------------------------------------------------------------

## Key Lesson

Requirements, design, and implementation cannot be treated as isolated
activities. Poor control at the requirements stage can propagate into
design, implementation, integration, testing, and ultimately production
failure.
