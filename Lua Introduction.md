# 📝 Introducing Luau 
This repost is where you can learn many diffrent codes about lua
for example 
```luau
print("Hello World");
```
As you can see the example i put was `print("Anything Here!");` if you make any mistake there will be some errors like if you dont use straight quotations like for example `print(”Error Found”);` that will cause the script to put a question mark symbol on any executor you use

## About the code `GetGenv():`
```luau
function getgenv(): { [string]: any }
```
It stands for "Get Global Environment". It returns a table representing the executor’s custom global environment. This allows you to create and access global variables, functions, and tables that persist across different scripts.

You can directly access global variables and functions stored in getgenv() without needing to use `getgenv().variableName`. For example, if a variable is stored as `getgenv().myVariable`, you can access it directly by just using `myVariable`.
However, if a local variable with the same name exists, the local variable will take precedence. In such cases, you must use `getgenv().variableName` to access the global variable.

## Examples on the code `GetGenv():`

```luau
--// Creating a new global variable \\--
getgenv().global_variable = "Hello, World!"
```
