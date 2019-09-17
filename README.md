
Introducción a R y análisis exploratorio de datos (AED o EDA)
=============================================================

Estudia este texto, y responde a los siguientes mandatos. Donde veas `...` debes colocar lo que corresponda para cumplir el mandato. **Teje tu documento sólo cuando hayas completado todos los mandatos y no te queden `...`**. Ejecuta tu código en la consola de R, línea a línea. Recuerda configurar `Chunck Output in Console`.

Ayuda de R
----------

-   Pide ayuda de todas las formas posibles sobre el paquete `vegan`.

``` r
help(package = '...')
library(help = '...')
```

-   Pide ayuda sobre la función `plot`.

``` r
help(...)
?
```

-   Pide un ejemplo de la función `plot`

``` r
example(...)
```

-   Busca la palabra clave `diversity` en los manuales y ayudas de R

``` r
help.search("...")
??
```

Carga conjuntos de datos
------------------------

### `doubs`

-   Carga el conjunto de datos `doubs`. Recuerda que éste pertenece al paquete `ade4` y primero tendrás que cargarlo a él

``` r
library(...)
data(...)
```

-   Despliega la matriz ambiental del conjunto de datos `doubs` (es un data frame denominado `env` dentro del conjunto `doubs`)

``` r
doubs$...
```

-   Explora la estructura de la matriz ambiental

``` r
str(...)
```

-   Despliega la matriz de comunidad del conjunto de datos `doubs` (es un data frame denominado `fish` dentro del conjunto `doubs`)

``` r
doubs$...
```

-   Explora la estructura de la matriz de comunidad

``` r
str(...)
```

-   ¿Cuántas filas tienen la matrices ambiental y de comunidad?

``` r
filasamb <- nrow(...)
filasamb
filascom <- nrow(...)
filascom
```

-   Selecciona la fila 15 de la matriz de ambiental y la misma fila de la matriz de comunidad

``` r
doubs$env[..., ]
doubs$fish[..., ]
```

-   En ambas matrices, ambiental y de comunidad, selecciona aleatoriamente la misma fila, y despliégala:

> La función `sample` elige números aleatorios a partir de un vector. Por ejemplo, `sample(1:100, 10)` elegirá `10` números aleatorios entre el `1` y el `100`. Si justo antes de ejecutar `sample` ejecutas `set.seed(x)` (sea `x` un número entero), la selección aleatoria será reproducible.

``` r
set.seed(10)
filaaleatoria <- sample(1:..., ...)
doubs$env[filaaleatoria, ]
doubs$fish[filaaleatoria, ]
```

### `mite`

-   Carga el conjunto de datos `mite`. La matriz de comunidad se denomina `mite` y la ambiental `mite.env`. Recuerda que este conjunto pertenece al paquete `vegan` y primero tendrás que cargarlo a él

``` r
library(...)
data(...) #Comunidad
data(...) #Ambiental
```

-   Despliega ambas matrices

``` r
...
...
```

-   Explora la estructura de la matriz ambiental

``` r
str(...)
```

-   Despliega la matriz de comunidad del conjunto de datos `doubs` (es un data frame denominado `fish` dentro del conjunto `doubs`)

``` r
doubs$...
```

-   Explora la estructura de la matriz de comunidad

``` r
str(...)
```
