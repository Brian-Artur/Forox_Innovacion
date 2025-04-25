---
Data: 2025-04-25
Language: TypeScript
---
# Void
Void significa que la función "no regresa nada". O que regresa *undefined*

![[Pasted image 20250425095334.png]]
Tenemos que usar un **: any** en tipado de la variable, si no sabemos qué valor le vamos a asignar a la función. Esto es por si vamos a reasignarle valores deferentes a posteriori. 

No tiene ningún sentido autoinvocar una función anónima si no se la va a guardar en una variable. A menos que sea algo tan simple como imprimir un *console.log()* en algún lado.

# Never
![[Drawing 2025-04-25 10.15.12.excalidraw|500]]
Se emplea el **never** para paralizar la ejecución del código. Algo así como utilizar un *break*. Suele ir dentro de un **catch**, del try-catch. Ya que lo que queremos es que "pete" la aplicación de forma controlada, si sucede alguna circunstancia. 

# Undefined
Tenemos que tener en cuenta qué valores vamos a devolver en un return de la función. Por eso, en un principio podemos decir que la función va a poder devolver un churro de tipos enorme. Pero que, a medida que vamos definiendo, y refactorizando la función, debemos cercar la cantidad de tipos que puede acabar devolviendo. 
![[Drawing 2025-04-25 11.16.07.excalidraw]]
# Enumeraciones 
![[Drawing 2025-04-25 13.15.13.excalidraw|500]]