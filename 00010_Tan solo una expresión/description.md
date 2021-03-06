Aunque no lo dijimos de manera explícita, seguramente ya te diste cuenta: las variables son también **expresiones**, y por lo tanto pueden usarse en los mismos lugares que todas las que ya conocías:

* como **argumentos** de funciones o procedimientos;
* en un `repeat`, indicando cuántas iteraciones hará;
* en un `if` o `while`, como parte de la condición;
* y como valor de retorno de una función.

Y claro, también pueden usarse en una **asignación**, o sea que ¡podemos asignarle un valor a una variable usando una variable! :fearful:

Veamos algunos ejemplos de esto que parece un trabalenguas:

```gobstones
algo := 25
cuantoVale := algo * 2
```
Nada muy nuevo, `algo` denota `25` y eso multiplicado por `2` vale `50`.

```gobstones
cuantoVale := Norte
cuantoVale := opuesto(cuantoVale)
```
Apa, acá hay que pensar un poco más. :frowning:
<br>
Al evaluar `opuesto(cuantoVale)`, la variable `cuantoVale` ya tenía el valor `Norte` y por lo tanto toda la expresión denotará `Sur`; eso será lo que finalmente será recordado bajo la etiqueta `cuantoVale`.

```gobstones
algo := 10
cuantoVale := 5
cuantoVale := (algo * cuantoVale) + cuantoVale
```

¿Y acá qué pasa?

> Este último caso te lo dejamos a vos, pensalo y escribí en el editor el valor al que etiqueta la variable. De nuevo, no tenés que escribir código Gobstones sino simplemente el número se obtendría al evaluar `cuantoVale` luego de todas las asignaciones.
