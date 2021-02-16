## Logical Condition

Use a defined convention to express logical expressions.

> Define a convention for logical expressions such as "[X AND Y]", "[X OR Y]", "[X XOR Y]", "NOT[X OR Y]".

#### Unacceptable

- The Engine_Management_System shall disengage the Speed_Control_Subsystem when the Cruise_Control is engaged, and the
Driver applies the Accelerator.

#### Acceptable

- The Engine_Management_System shall disengage the Speed_Control_Subsystem, when [the Cruise_Control is engaged AND the
Driver applies the Accelerator].