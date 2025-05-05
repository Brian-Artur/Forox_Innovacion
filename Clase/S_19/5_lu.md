# Relation vs Relationship
#SQL 
## Relation (Relación como "tabla")
En bases de datos, una **relation** es una **tabla**.  
Cada tabla tiene filas y columnas.
- Las **filas** (también llamadas _registros_ o _tuplas_) representan datos individuales.
- Las **columnas** (también llamadas _atributos_) representan las características de esos datos.
## Relationship (Relación entre tablas)
Una **relationship** es una **relación entre dos o más tablas**.  
Sirve para conectar datos que están en diferentes tablas. No tiene que ser mediante una tabla intermedia. Cualquier relación que se haga entre clave primaria y clave foránea, es un relationship.

Ejemplo:  
Supón que tienes dos tablas:
- **Estudiantes** (`ID`, `Nombre`, `Edad`)
- **Cursos** (`ID`, `NombreCurso`)
Y una tercera tabla:
- **EstudiantesCursos** (`ID_Estudiante`, `ID_Curso`)
Esa tercera tabla crea una **relationship** entre _Estudiantes_ y _Cursos_.  
Es decir: conecta qué estudiante está en qué curso.

## Dominio 
El dominio de un atributo 

## Producto cartesiano de los dominios

## Relación = subconjunto del producto cartesiano


# Relaciones
## Desglosar 1 tabla en muchas
![[Drawing 2025-05-05 14.14.21.excalidraw|500]]
Fragmentamos una tabla con muchas columnas en muchas tablas con pocas columnas. Estas tablas van a estar relacionadas por `1:1` porque necesitamos que haya exactamente la misma cantidad 

# Objetos
#TypeScript 
En JavaScript podemos añadir nuevas propiedades a un objeto. E incluso pisar el objeto que ya hemos creado. Cosa que es TS nos va a señalar error, pese a que nos termine permitiendo.
![[Pasted image 20250505100307.png|550]]
Cuando estamos definiendo el objeto por primera vez, aunque no lo estemos tipando explícitamente. Estamos creando un nuevo tipo basado en el propio objeto y sus propiedades.
TypeScript infiere por nosotros los tipos de datos que hay en ese objeto.

Podemos aplastar todo el objeto ya creado. Siempre y cuando le asignemos valores a TODAS las propiedades.
## This
Todo objeto tiene un apuntador que apunta a sí mismo para evitar un problema.

Un método con función de flecha NO IMPLEMENTA (hereda) `this`
![[Drawing 2025-05-05 10.16.29.excalidraw]]

## Getter
El Get lo que hace es mostrarte los que hay en el interior de un objeto.

Es horrible encontrarse un objeto plagado de Getters y Setters.

Es una buena práctica el tener un Getter que actúe como valadador de los datos que hay dentro del mismo objeto.

# Docker
![[Drawing 2025-05-05 12.10.29.excalidraw|450]]

# Objetos tipados
A la hora de tipar las funciones, debemos ser más específicos y decir qué parámetros va a tener y qué tipo de valor va a devolver. Colocar sólamente el tipo Function (constructor de funciones) no es aconsejable; ya que da demasiada libertad a TS.
![[Drawing 2025-05-05 12.34.32.excalidraw]]
Como programador debes estar consciente al 100% de los que haces

Al ser Opcional la función, sabes que puede retornar UNDEFINED. Pero tú sabes que esta nunca lo hará.

# Trazabilidad
Es importante seguir la trazabilidad; ya que podremos dale pasos atrás. Para hacer este proceso lo que hacemos es crear un nuevo objeto para cada versión.

Por eso no es bueno modificar un objeto ya creado. Pues no vamos a saber qué es lo que había en un pasado en ese objeto.
![[Drawing 2025-05-05 12.46.16.excalidraw|600]]

# Type
Palabra reservada para definir nuevo tipo de dato.
![[Drawing 2025-05-05 13.15.07.excalidraw|250]]
Puedes utilizar indistintamente `;` o `,`.

# Preguntar a ChatGPT
1. Decir que actúe como un expertor en el tema.
2. Le preguntamos sobre nuestra duda.
3. Si no lo entendemos. Copiamos su respuesta y le planteamos nuestra duda acerca de eso.

# Normalizaciones
El kit está en asegurar que no haya datos duplicados. Que la BBDD ocupe lo mínimo y sea más rápida.
![[Drawing 2025-05-05 14.37.05.excalidraw]]
## 1FN

> Si vamos a sacar un certificado de Oracle debemos ssaber qué signifacan esas relaciones teoricas de `0:1` . Lo mismo pasa con las formas normales, que en la vida real solo se emplean hasta la 3ª forma normal. Pero si queremos ser expertos, sí que debemos conocer las 8 (la última no se sabe si está terminada).


# Tareas
- [ ] Buscar formas de hacer copia profunda.
- [ ] Cómo hacemos que en un objeto, una función retorne algo por defecto; sin haberselo asignado.
- [ ] Escribir las primeras 3FN