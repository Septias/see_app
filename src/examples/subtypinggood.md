```ocaml
let hlist: shape list = [(square 10 :> shape); (circle 30 :> shape)];;
val hlist : shape list = [<obj>; <obj>]
let shape_ref: shape ref = ref (square 40 :> shape);;
val shape_ref : shape ref = {Base.Ref.contents = <obj>}
shape_ref := (circle 20 :> shape);;
- : unit = ()
```