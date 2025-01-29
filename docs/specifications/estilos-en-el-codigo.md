# Guía de estilos

## Técnica para elegir nombres

**¿Cómo elegir buenos nombres?**
- Fáciles de pronunciar.
    - No utilizar el guion bajo, "underscore". ❌
    - No utilizar convenciones o notaciones de otra era como la "hungara". ❌
    - No comerse letras en las palabras para acortarlas. ❌
    - Un nombre demasiado largo puede indicar que la abstracción no es buena.
    - Los índices de los bucles pueden ser la excepción y utilizar i, j, k. ✅
- Sin información técnica.
    - Evitar que diga que el tipo de una variable es *string, interface, clase abstracta, implementación de una interface, etc...*
        ```java=
        sSurname, IShoppingCart, AbstractShoppingCart, ShoppingCartImpl, IAsyncUserFinder,…
        ```
    - La dificultad para ponerle nombre a una interfaz te está diciendo que no necesitas que exista esa interfaz. 👀
    - Excepciones:
        - Dto, para los objetos de transporte de datos.
        - Repository, para las clases que implementan dicho patrón de Domain-driven design.
        - ViewModel, para los objetos que modelan vistas.
    - ¿Para que es? ✅ Esta es la pregunta que debemos hacernos.
    - ¿Como está implementado? ❌ La implementación no debe estar descrita en los nombres.
- Nombres concretos.
    - Si un nombre es aplicable a muchos elementos a la vez, debamos descartarlo. ❌
        ```java=
        Helper, manager, generator, engine, tool, service, utils, process, execute, input, …
        ```
    - Evitar los nombres que valen para todo.
    - Excepciones:
        - execute, cuando implementamos un patrón command.
        - service, cuando nos apoyamos en Domain-driven design.
- Nombres que formen frases.
    - Utilizar prefijos de tipo pregunta, para expresiones o variables tipo boolean:
        - is, has, does, are, contains, will, should…
    - Incluso a veces se utilizan las negaciones:
        - isNot, doesnt, hasnt…
    - No son recomendables los operadores lógicos: ❌
        - and y or, denotan exceso de responsabilidad.
        ##### Ejemplo:
        ```java=
        saveUserAndSendEmail()
        ```
        El método saveUserAndSendEmail() realiza dos acciones a la vez. Si las dos acciones han de realizarse en bloque, seguramente existe un nombre de dominio más adecuado para la operación.
        ##### Ejemplo:
        ```java=
        registerUser()
        ```
    - Mejor utilizar los propios operadores del lenguaje, ya que cuando son parte de un nombre denotan exceso de responsabilidad.