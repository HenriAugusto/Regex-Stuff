# Enforce proper name format

`^([[:upper:]][[:lower:]]+ )([[:upper:]]([[:lower:]]*|\.) )*([[:upper:]][[:lower:]]+$)`

- Names will have to always be in proper case
- there shouldn't be any leading or trailing whitespaces
- no double spaces between surnames
- last name cannot be abbreviated

### Should Match

Alberto Bruno C Daniel E F Giordano
Alberto Bruno C Daniel E F. Giordano

### Should NOT Match

Alberto
A Bruno C
Alberto Bruno C Daniel E F. G
A. Bruno C Daniel E F. Giordano
Alberto Bruno C DOUBLE  SPACE E F Giordano
 Leading Whitespace Alberto Bruno C Daniel E F Giordano
Trailing Whitespace Alberto Bruno C Daniel E F Giordano 

## No abbreviations Variations

`^([[:upper:]][[:lower:]]+ )([[:upper:]][[:lower:]]+ )*([[:upper:]][[:lower:]]+$)`
