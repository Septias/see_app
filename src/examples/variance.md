```ocaml
let squares: square list = [ square 10; square 20 ];;
val squares : square list = [<obj>; <obj>]

// diese coercion ist nur möglich, da der `Listtyp` immutable ist
let shapes: shape list = (squares :> shape list);;
val shapes : shape list = [<obj>; <obj>]
```