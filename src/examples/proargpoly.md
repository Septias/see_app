```ocaml
let remove_large l =
List.filter ~f:(fun s -> Float.(s#area <= 100.)) l;;
val remove_large : (< area : float; .. > as 'a) list -> 'a list = <fun>

let squares : < area : float; width : int > list =
[square 5; square 15; square 10];;
val squares : < area : float; width : int > list = [<obj>; <obj>; <obj>]
remove_large squares;;
- : < area : float; width : int > list = [<obj>; <obj>]
```