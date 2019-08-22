### pug2
createElement engine, like a pug.

```fragment=pug2(string)```

```
//pug2
//one line be the one element setting.
let fr=pug2(`
.col1
 .a 
  .a1
  .a2
  .a3
//comment is silent.  
 .b
 .c
.col2
 .d
 .e
 .f
`);

//space is back parentElement

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


### complete pattern
```
.frame(data-mode="WIP" data-close="false" data-id="###")
 .wrap.bar
  .cap.single(contenteditable="true") captionThis
  .stt(onclick="stt(event)" data-text="20190821 WIP)
  .clo(onclick="clo(event)" data-text="	-")
 .wrap.editor
  .num.wipe 000
  .ed(contenteditable="plaintext-only" onkeyup="ed(event)") its new
```

