# TallerEspecificidadCSS

Parte 1: Introducción Teórica a la Especificidad

1. ¿Qué es la especificidad?

La especificidad es una regla que utiliza el cliente (navegador) para determinar qué estilos aplicar en caso de que existan conflictos entre diferentes reglas CSS.

Cuando múltiples selectores afectan el mismo elemento, el cliente asigna "puntos" a cada selector para decidir cuál es más específico. La regla con mayor cantidad de puntos se aplicará, asegurando que el CSS sea predecible y controlable, es decir, se podrá definir que estilo aplicar teniendo en cuenta los puntos de especificidad.

2. Reglas de cálculo de especificidad:

| Selector          |     Puntuación de especificidad                                                       |
-------------------------------------------------------------------------------------------------------------
|Style = “en línea” |Supera la especificidad                                                                |
|#nombre “ID”       |100                                                                                    |
|.nombre “Clase”    |10                                                                                     |
|nombre “Etiqueta”  |1                                                                                      |
|!important         |fuerza que la regla CSS sea aplicada, ignorando la especificidad y el estilo en línea. |

Parte 2: Ejemplos Prácticos

1. Ejemplo básico:

2. Demostración de !important:


Parte 3: Ejercicios Prácticos

Ejercicio 1: Calculando la Especificidad

¿Qué color tendrá el título <h1>?
El titulo tendra color rojo debido a que se esta aplicando el estilo por ID con puntaje de especificidad de 101.

Ejercicio 2: Resolviendo Conflictos de Especificidad


El titulo cambia de color a amarillo debido a que se  aplica adicionalmente al estilo por ID un estilo por clase .text lo cual sube el puntaje de especificidad de 101 a 110, por lo tanto, no es necesario usar el !important.

Parte 4: Desafío Final

Desafío: Diseñando una Página Completa con Estilos Conflictivos

Desafío CSS:
El <h1> en el .header debe ser de color blanco.
El texto del <p> en .content debe ser rojo.
El texto del <footer> debe ser gris.

