# FMUL

<PageHeader />  

**Tags:**
<badge text='mathematical operations' vertical='middle' />
<badge text='floating point operations' vertical='middle' />

## Description

This function performs floating point mutiplication on two numeric values.

It takes the general form:

```
FMUL(expression1, expression2)
```

where both **expression1** and **expression2** must evaluate to non-null numeric values.

## Note

> If either of the arguments evaluates to null then a run time "non-numeric" error will occur.
> The calculation is not subject to the [PRECISION](./../precision) setting.

An example of use would be as:

```
CRT FMUL(4.0017, -1.83)
```

to display '-7.323111'.

Go back to [jBASE BASIC](./../README.md)

Go back to [Programmers' Reference Guide](./../../reference-guides/jbc/README.md)

<PageFooter />
