# SDLC Failure Mapping: Healthcare.gov

## Objective

The purpose of SDLC failure mapping is to identify:

1.  Where each major failure originated in the Software Development Life
    Cycle (SDLC).
2.  Where the problem was later detected.
3.  The category of failure associated with it.

This distinction is important because a problem may originate in one
SDLC phase but remain undetected until testing or production.

## Failure Mapping

  ----------------------------------------------------------------------------------
                No. Major Technical  SDLC Origin      Detection     Failure Category
                    Cause            Phase            Phase         
  ----------------- ---------------- ---------------- ------------- ----------------
              **1** Requirements     Requirements     Testing /     **C1 ---
                    were not                          Development   Requirements
                    effectively                       Review        Failure**
                    managed and were                                
                    not consistently                                
                    approved or                                     
                    linked to                                       
                    lower-level                                     
                    requirements.                                   

              **2** Planned          Requirements /   Testing /     **C1 / C4**
                    functionality    Implementation   Production    
                    was not                                         
                    completely                                      
                    implemented                                     
                    before the                                      
                    initial launch.                                 

              **3** Software coding  Implementation   Testing /     **C4 ---
                    errors were                       Production    Implementation
                    identified but                                  Failure**
                    were not                                        
                    adequately                                      
                    corrected before                                
                    launch.                                         

              **4** Healthcare.gov   Testing          Production /  **C5 --- Testing
                    and supporting                    User          & Verification
                    systems were not                  Experience    Failure**
                    fully tested                                    
                    before launch.                                  

              **5** Test             Testing          Testing       **C5 --- Testing
                    documentation                     Review        & Verification
                    did not contain                                 Failure**
                    sufficient                                      
                    information to                                  
                    properly                                        
                    determine                                       
                    whether tests                                   
                    had passed or                                   
                    failed.                                         

              **6** The system was   Requirements /   Production    **C2 / C3**
                    not adequately   Design                         
                    planned for the                                 
                    expected                                        
                    workload and                                    
                    capacity                                        
                    requirements.                                   
  ----------------------------------------------------------------------------------

## Important Observation

The mapping shows that several problems were detected later than the
phase in which they originated.

For example:

-   Capacity planning originated in **Requirements / Design**, but its
    consequences were detected in **Production**.
-   Implementation problems were identified during **Testing /
    Production**.
-   Requirements problems were exposed through **Testing / Development
    Review**.

This indicates weaknesses in early verification and validation.

## SDLC Breakdown

### Requirements Phase

Problems included ineffective requirements management and insufficient
control of system expectations.

### Design Phase

Capacity and workload requirements were not adequately planned.

### Implementation Phase

Planned functionality was incomplete and coding errors remained
unresolved.

### Testing Phase

Testing was incomplete, and test documentation was insufficient to
establish clear pass/fail outcomes.

### Production

The consequences became visible through outages, errors, slow
performance, and inability to reliably handle real-world demand.

## Key Lesson

A strong SDLC should detect problems as close as possible to their
origin. When requirements, design, implementation, and testing problems
survive until production, the cost and impact of correction increase
substantially.
