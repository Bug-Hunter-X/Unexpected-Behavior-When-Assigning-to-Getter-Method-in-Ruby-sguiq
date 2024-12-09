# Unexpected Behavior When Assigning to Getter Method in Ruby

This repository demonstrates an uncommon Ruby bug related to assigning values to getter methods.  Direct assignment to a getter method does not modify the underlying instance variable.  This behavior can be unexpected for programmers unfamiliar with Ruby's conventions.

The `bug.rb` file shows the erroneous behavior. The `bugSolution.rb` file shows a corrected version that uses a setter method to update the instance variable.

**Problem:**
Attempting to update an instance variable directly via the getter method doesn't work as expected.

**Solution:**
Define a setter method (`value=`) to properly update the instance variable.