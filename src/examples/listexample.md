```ocaml
let hlist: < area: float; ..> list = [square 10; circle 30];;
Line 1, characters 50-59:
Error: This expression has type < area : float; radius : int >
       but an expression was expected of type < area : float; width : int >
       The second object type has no method radius
```