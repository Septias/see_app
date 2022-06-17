```ocaml
open Base;;
let s = object
  val mutable v = [0; 2]

  method pop =
    match v with
    | hd :: tl ->
      v <- tl;
      Some hd
    | [] -> None

  method push hd =
    v <- hd :: v
end;;
val s : < pop : int option; push : int -> unit > = <obj>
```