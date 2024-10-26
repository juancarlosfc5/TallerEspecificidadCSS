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

[**Diapositivas**] (https://github.com/juancarlosfc5/TallerEspecificidadCSS/blob/ef7d54f7edac569172d6cd2b9aab8462e6c7b3bd/Parte1/Especificidad.pptx)

Parte 2: Ejemplos Prácticos

1. Ejemplo básico:
![2 1 1](https://github.com/user-attachments/assets/ff92057a-fc7d-4bca-a7c1-1766e9236ebb)
![2 1 2](https://github.com/user-attachments/assets/abc932eb-f3d9-48e8-b1f7-f44a186d870e)
![2 1 3](https://github.com/user-attachments/assets/5ae30f6c-74a4-4ead-80d4-0466d3bf7dc9)

2. Demostración de !important:
![2 2 1](https://github.com/user-attachments/assets/8e3d2c89-a49c-422c-930e-42fad103c71c)
![2 2 2](https://github.com/user-attachments/assets/590caed1-2abc-4fc4-8b32-2bba4b8b3740)
![2 2 3](https://github.com/user-attachments/assets/99271be7-222a-4043-a43a-43f75358a24a)

Parte 3: Ejercicios Prácticos

Ejercicio 1: Calculando la Especificidad
![3 1 1](https://github.com/user-attachments/assets/fffade40-a6e8-4fdf-a766-4eaf82859270)
![3 1 2](https://github.com/user-attachments/assets/2a9f141c-2081-4785-82e3-510aa094a668)
![3 1 3](https://github.com/user-attachments/assets/990d59b3-e4fa-41ab-9bb6-aa26ee791ce7)

¿Qué color tendrá el título <h1>?
El titulo tendra color rojo debido a que se esta aplicando el estilo por ID con puntaje de especificidad de 101.

Ejercicio 2: Resolviendo Conflictos de Especificidad
![3 2 1](https://github.com/user-attachments/assets/6156663f-ce1c-4e36-9744-660a6045673a)
![3 2 2](https://github.com/user-attachments/assets/66e1859d-2a4c-4e17-841d-d3a8059f6a81)
![3 2 3](https://github.com/user-attachments/assets/e474b966-2f09-4055-bf03-667efbcc0a94)


El titulo cambia de color a amarillo debido a que se  aplica adicionalmente al estilo por ID un estilo por clase .text lo cual sube el puntaje de especificidad de 101 a 110, por lo tanto, no es necesario usar el !important.

Parte 4: Desafío Final

Desafío: Diseñando una Página Completa con Estilos Conflictivos
![4 1 1](https://github.com/user-attachments/assets/1d226126-2f18-4c83-9f89-190ebaeb52fe)
![4 1 2](https://github.com/user-attachments/assets/4bae143e-7f72-4a8c-900c-a003e80904c6)

Desafío CSS:
El <h1> en el .header debe ser de color blanco.
![4 1 3](https://github.com/user-attachments/assets/ffc263f0-83ae-469b-a17a-d3789d2cbdfb)
Se usa la especificidad de ID y etiqueta para lograr un puntaje de 101 y que aplique solo al titulo.

El texto del <p> en .content debe ser rojo.
![4 1 4](https://github.com/user-attachments/assets/24345dee-5700-4f87-bb19-b0f0eea28293)
Se usa la especificidad de clase para lograr un puntaje de 10 y que aplique al contenedor.

El texto del <footer> debe ser gris.
![4 1 5](https://github.com/user-attachments/assets/0100eb45-48f2-451f-96de-c2cd1c427bab)

Se usa la especificidad de ID para lograr un puntaje de 100 y que aplique a todo el footer.
