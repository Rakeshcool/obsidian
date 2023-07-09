#sytax
- declaring a variable use syntax : var *variable_name* datatype
- short assignment :  *:=*
- for example :{ syntax: congrats := "happy birthday!" }
# CONSTANTS

Constants are declared like variables but use the `const` keyword. Constants can't use the `:=` short declaration syntax.

Constants can be character, string, boolean, or numeric values. They _can not_ be more complex types like slices, maps and structs, which are types we will explain later.

As the name implies, the value of a constant can't be changed after it has been declared.

## USE TWO SEPARATE CONSTANTS

Something weird is happening in this code.

What _should_ be happening is that we create 2 separate constants: `premiumPlanName` and `basicPlanName`. Right now it looks like we're trying to overwrite one of them.