# Ruby Instance Variable Hiding Bug

This repository demonstrates a subtle bug in Ruby where a method's name clashes with an instance variable, preventing modification of the instance variable through the method.

The `bug.rb` file contains the buggy code.  The `bugSolution.rb` file provides a corrected version.

## Bug Description

When a method is defined with the same name as an instance variable, the method effectively hides the instance variable. Any attempts to assign a value using the method name will create a local variable within the method's scope, not modify the instance variable.