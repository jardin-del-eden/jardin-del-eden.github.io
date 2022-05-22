# Blog de Ejemplo

Este es un blog automáticamente generado, es decir, lo hice yo pero no es necesario programar nada - se puede generar a partir de texto plano

la apariencia es solo una plantilla pero se puede mejorar muchisimo - vosotros solo decidme y se lo puedo integrar sin ningun problema, incluso dar estilos personalizados o ambientes a cada blog acordes a su tema

ahora ejemplos de cosas :

## Un subtitulo

un poco mas de texto

### Y un subtitulo de un subtitulo???

#### Hasta donde podemos llegar?

##### Creo que ya está bien de subtitulos

```rust

/* Algorithm to calculate the digital root of a number
> Digital root -> the sum of the digits of a number untill the number of digits is equal to 0
    16  -->  1 + 6 = 7
   942  -->  9 + 4 + 2 = 15  -->  1 + 5 = 6
132189  -->  1 + 3 + 2 + 1 + 8 + 9 = 24  -->  2 + 4 = 6
493193  -->  4 + 9 + 3 + 1 + 9 + 3 = 29  -->  2 + 9 = 11  -->  1 + 1 = 2
*/

const RADIX: u32 = 36;

fn digital_root(n: i64) -> i64 {
    let mut s: String = n.to_string();
    while s.chars().count() != 1 {
        let mut v: Vec<i64> = Vec::new();
        for ch in s.chars() {
            let int = ch.to_digit(RADIX).unwrap();
            v.push(int as i64);
        }
        let sum: i64 = v.iter().sum();
        s = sum.to_string();
    }
    return s.parse().unwrap();
}

fn main() {
    let n: i64 = 942;
    let result: i64 = digital_root(n);
    println!("{} --> {}", n, result);
}
```

Un algoritmo con syntax highlighting porque a quien no le gusta eso -> aunque no creo que este os sirva de mucho

[un link](https://www.youtube.com/watch?v=dQw4w9WgXcQ) para hacer lo que sea que hagan los links

[y el codigo fuente de esta pagina](https://github.com/jardin-del-eden/jardin-del-eden.github.io) por si alguien quiere verlo o modificarlo

un poco de texto en **negrita** para que se vea mejor o incluso en *italica* porque no?

> una frase super importante

- una lista
- de elementos
- desordenados

1. y una
2. de elementos
3. desordenados
