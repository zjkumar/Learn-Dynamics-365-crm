- _The most common scenario is to verify null values and default it to a specific value._
- _It can be achieved using Coalesce function_.
- _It evaluates a list of arguments in order and returns the first non-null or non-blank value it encounters._


### Understanding the syntax :-

```
The syntax coalesce(variables('Plan') ? ['plantype'], false) is used in Power Automate to handle null or undefined values. Let’s break it down step by step:

Breakdown of the Syntax
variables('Plan'):
This part retrieves the value of a variable named Plan in your flow.
variables('Plan') ? ['plantype']:
The ? operator is a shorthand for the conditional (ternary) operator in some programming languages, but in Power Automate, it is used to safely access properties of an object.
variables('Plan') ? ['plantype'] checks if the Plan variable is not null or undefined and then tries to access the plantype property of the Plan object.
```