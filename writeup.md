# Lab 6 Writeup
#### Drew Casner

3bi) 
```
       re ::= union
    union ::= union `|` intersect | intersect
intersect ::= intersect & concat | concat
   concat ::= concat not | not
      not ::= ~ not | star
     star ::= star* | star+ | star? | atom
     atom ::= ! | # | . | c
```

3bii)

3biii)
```
       re ::= union
    union ::= intersect {`|` intersect}
intersect ::= concat {`&` concat}
   concat ::= not {not}
      not ::= {~} star
     star ::= atom | atom {*} | atom {+} | atom {?}
     atom ::= ! | # | . | c
```

3biv)
```
        re ::= union
     union ::= intersect unions
    unions ::= € | `|` intersect unions
 intersect ::= concat intersects
intersects ::= € | `&` concat intersects
    concat ::= not concats
   concats ::= € | not concats
       not ::= nots star
      nots ::= € | `~` nots
      star ::= atom stars
     stars ::= € | stars {*} | stars {+} | stars {?}
      atom ::= ! | # | . | c | `(`re`)`
```

3c)
