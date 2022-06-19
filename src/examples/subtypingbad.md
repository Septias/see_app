```ocaml
let remove_large (l: < area : float > list) =
List.filter ~f:(fun s -> Float.(s#area <= 100.)) l;;
val remove_large : < area : float > list -> < area : float > list = <fun>
remove_large (squares :> < area : float > list );;
- : < area : float > list = [<obj>; <obj>]

```