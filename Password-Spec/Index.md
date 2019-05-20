## Password-Spec

Password-Spec is a specification for including password metadata
in the HTML source so password managers and browsers can provide
guidance to the user on how to set the password.

The meta-data would include values such as minimum length, maximum length,
required characters and invalid or restricted characters.

### Example 1

This site has a minimum length of 8 characters and a maximum of 32,
permits only alphanumeric characters.
```html
<input type="password" password-spec="min:8,max:32,valid:alpha" />
```

### Example 2

This site permits a mimimum of six chars and no maximum. Any character is allowed
but must contain at least 1 upper case, 1 lower case, 1 number and one special character
```html
<input type="password" password-spec="min:8,max:32,valid:any,minupper:1,minlower:1,minnumber:1,minspecial:1" />
```
