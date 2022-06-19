```ocaml
type shape = < variant : repr >
and circle = < variant : repr; radius : int >
and line = < variant : repr; length : int >
and repr =
 | Circle of circle
 | Line of line;;
type shape = < variant : repr >
and circle = < radius : int; variant : repr >
and line = < length : int; variant : repr >
and repr = Circle of circle | Line of line
let is_barbell = function
| [s1; s2; s3] ->
   (match s1#variant, s2#variant, s3#variant with
    | Circle c1, Line _, Circle c2 when c1#radius = c2#radius -> true
    | _ -> false)
| _ -> false;;
val is_barbell : < variant : repr; .. > list -> bool = <fun>
```