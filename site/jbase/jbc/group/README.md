# GROUP

<PageHeader />  

**Tags:**
<badge text='grouping' vertical='middle' />

## Description

The **GROUP** function is equivalent to the [FIELD](./../field) function. It takes the general form:

```
GROUP(Expression1, Expression2, Expression3, Expression4)
```

Where:

- **Expression1** evaluates to the string containing fields to be extracted,
- **Expression2** evaluates to the character(s) delimiting each field within **Expression1,**
- **Expression3** should evaluate to a numeric value specifying the number of the first field to extract from **Expression1,**
- **Expression4** evaluates to a numeric value specifying the number of fields to extract as a group.

## Note

> **Expression2** may evaluate to more than a single character allowing fields to be delimited with complex expressions.

An example of use is as:

```
num_List = "123:-456:-789:-987:-"
CRT GROUP(num_List, ":-", 2, 2)
```

to display:

```
-456:-789
```

on the terminal, being the second and third fields and their delimiter within variable num_List .

Go back to [jBASE BASIC](./../README.md)

Go back to [Programmers' Reference Guide](./../../reference-guides/jbc/README.md)
  
<PageFooter />
