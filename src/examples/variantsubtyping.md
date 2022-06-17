
```ocaml
type num = [ `Int of int | `Float of float ];;
type num = [ `Float of float | `Int of int ]
type const = [ num | `String of string ];;
type const = [ `Float of float | `Int of int | `String of string ]
let n : num = `Int 3;;
val n : num = `Int 3
let c : const = (n :> const);;
val c : const = `Int 3
```
