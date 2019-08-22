# pug2
createElement engine, like a pug.

```fragment=pug2(string)```

```
//pug2

let fr=pug2(`
.col1
 .a 
  .a1
  .a2
  .a3
 .b
 .c
.col2
 .d
 .e
 .f
`);

pug2(fr).a2('body') //append to body

```
chain

```pug2(...).a2(query)```

```
//appends
pug2(...).a2(parent) //append to
pug2(...).p2(parent) //prepend to
pug2(...).as(parent) //append siblings to
pug2(...).ps(parent) //prepend siblings to
pug2(...).rep(alive) //replace target the alive, within body only.
```
