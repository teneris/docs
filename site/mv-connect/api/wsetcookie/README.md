# WSETCOOKIE

<PageHeader />

The WSETCOOKIE subroutine will set a cookie to be sent back to the browser.

## Command Sytax

```
CALL WSETCOOKIE(NAME,VALUE,EXP.DATE,EXP.TIME,PATH,DOMAIN,SECURE)
```

### Syntax Elements

| <!----> | <!----> |
| --- | --- |
| NAME | Name of the cookie you want to set |
| VALUE | Value you wish to set the cookie to |
| EXPDATE | Date you wish the cookie to expire on.  Use pick internal dates. |
| EXPTIME | Time you wish the cookie to expire (used with EXPDATE).  Use pick internal times. |
| PATH | Path you wish the cookie to apply to.  Use "/" for all. |
| DOMAIN | Domain you wish the cookie to apply to.  Use "." for domain called from. |
| SECURE | If set to "Y" then this cookie will only save on HTTPS requests. |

#### Example

```
CALL WSETCOOKIE("mycookie","value",DATE(),TIME+300,"/",".","Y")
```

#### Notes

The WSETCOOKIE command basically builds a Set-Cookie header.  This function properly formats the Set-Cookie for you and understands pick date and time formats.  If you wish more control you can use the WSETHEADER and build your own Set-Cookie line.

Here is a good [link](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie "Link to Set-Cookie documentation") on how Set-Cookie works.

<PageFooter />
