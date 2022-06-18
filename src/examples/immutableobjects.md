```ocaml
let imm_stack init = object
  val v = init

  method pop =
    match v with
    | hd :: tl -> Some (hd, {< v = tl >})
    | [] -> None

  method push hd =
    {< v = hd :: v >}
end;;
val imm_stack :
  'a list -> (< pop : ('a * 'b) option; push : 'a -> 'b > as 'b) = <fun>
```