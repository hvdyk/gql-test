# Issue List
## Psiber 
### AGT600 - Master Data
* PAYROLL NAME max length = 16
* Blank fields (not used): DEPARTMENT, DIVISION, PAYPOINT
* Blank fields (need naming convention): COST CENTRE
  Require final decision if this should be blank
* Job Grade and Job Title
   * Static data - waiting for confirmation of lengths of the name field
   * AGT mapping - ToDo
* Bank   
   * Bank Branch Code: Remove leading 2 zero’s for all
   * Bank Account Number(#): IF VAL(#)>=10 THEN VAL(#) ELSE RIGHT(#,11)
* Tax Overrides
   * Where TAX OVERRIDE METHOD = 4, and there is a TAX OVERRIDE PERCENTAGE, but no TAX DIRECTIVE NUMBER and/or TAX OVERRIDE EFFECTIVE DATE – Defaulted the values to TAX DIRECTIVE NUMBER = 000000 and TAX OVERRIDE EFFECTIVE DATE = 20170301. 
* UIF OVERRIDE (Is Y and N): 
   * Should this be set to N and be controlled by the Package Template?
### AGT603 – Medical Aid Package
* Verify with MK that the list is now correct.
* GG to make changes 
### AGT605 – Master Information Pay
* Change default from <blank> to ...:
   * MONTHS ON SCHEME WITH PREVIOUS EMPLOYER(S) = 0
   * TAKE ON ETI MONTHS WITH CURRENT EMPLOYER = 0
   * TAKE ON ETI REMUNERATION WITH CURRENT EMPLOYER = 0
   * TAKE ON ETI VALUE WITH CURRENT EMPLOYER = 0
   * ASYLUM SEEKER = N
   * MONTHLY MINIMUM WAGE = 0
### AGT608 - Package Information
* Change specification in code
### AGT626 Custom Fields
* Change Cover Income
   * V02SALDO [V02TSALD=L] / 1000 
* Waiting for new custom fields to be added, before handing over to development.
### AGT627 - Dependent Details
