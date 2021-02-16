## Explicit Lists

Express the propositional nature of a condition explicitly for a single action instead of giving lists of actions for a
specific condition.

> When a list of conditions is given for a single action in a single need or requirement statement, it may not be clear
whether all the conditions must hold (a conjunction) or any one of them (a disjunction) for the action to take place.

#### Unacceptable

* The Audit_Clerk shall be able to change the status of the action item when:
    * the Audit_Clerk originated the item;
    * the Audit_Clerk is the actionee; and
    * the Audit_Clerk is the reviewer.

#### Acceptable

* Acceptable if interpreted as a disjunction: The Audit_System shall allow the Audit_Clerk to change the status of the
action item when one or more of the following conditions hold:
    * the Audit_Clerk originated the item;
    * the Audit_Clerk is the actionee;
    * the Audit_Clerk is the reviewer.
    
* Acceptable if interpreted as a conjunction: The Audit_System shall allow the Audit_Clerk to change the status of the
action item when the following conditions are simultaneously true:
    * the Audit_Clerk originated the item; and
    * the Audit_Clerk is the actionee; and
    * the Audit_Clerk is the reviewer.