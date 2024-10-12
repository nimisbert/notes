## Keywords
- Variable immuable:
```RUST 
let x = 5;
x = 6; // erreur
```
- Variable mutable:
```Rust
let mut x = 5;
x = 6; // ok
```
- Constantes:
```Rust
const THREE: u32 = 3;
```
- Shadowing:
```Rust
let x = 5;
let x = 6; // ok
```
Mais le type n'est pas mutable.
- Types:
```Rust
let x = 2.0;      // f64
let y: f32 = 2.0; // f32
```
- Tuples:
```Rust
let tup: (i32, f64, u8) = (500, 2.0, 1);
let (x,y,z) = tup;
let five_hundred = tup.0;
```
- Array:
```Rust
let a = [1,2,3,4,5];
let b: [i32; 5] = [1,2,3,4,5];
let c: [3; 3]; // [3,3,3]
let first = a[0];
let last = a[4];
```
- Fonctions:
```Rust
fn foo(x: i32) {
}
```
- Déclaration:
```Rust
let y = {
	let x = 3;
	x + 1;
} // y = 4
```
- Retours:
```Rust
fn bar() -> i32 {
	42
}
```
