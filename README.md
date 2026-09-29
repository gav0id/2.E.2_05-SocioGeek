Ejercicio 2.E.2 05 - Socio Geek

Lógica del programa
Para resolver este ejercicio del Bloque III, me enfoqué en aplicar el principio de encapsulamiento y protección del estado interno (information hiding). Diseñé la clase `SocioGeek` y definí sus tres atributos (`numeroSocio`, `nombre` y `puntosFidelidad`) utilizando el modificador de acceso `private`.

Para inicializar los objetos, implementé un constructor parametrizado. Como los atributos son privados, proporcioné métodos *getters* para permitir la lectura externa de cada uno de ellos. 

El punto central de este ejercicio fue la creación de un método *setter* con validación defensiva para los puntos de fidelidad. Implementé `setPuntosFidelidad(int puntosFidelidad)` utilizando una estructura condicional (`if/else`) que evalúa el dato entrante: si el valor es mayor o igual a cero, se actualiza el atributo; de lo contrario, se rechaza la modificación y se imprime un mensaje de error advirtiendo que los puntos no pueden ser negativos.

Dentro de la clase `Main`, implementé la lógica de prueba:
1. Instancié un objeto `SocioGeek` con datos iniciales válidos (67 puntos de fidelidad).
2. Imprimí el estado inicial utilizando los métodos *getters*.
3. Intenté forzar un estado inválido llamando a `setPuntosFidelidad(-15)`.
4. Volví a imprimir el estado del objeto. Esto me permitió comprobar por consola que el mensaje de error se dispara correctamente y que el valor de los puntos de fidelidad originales (67) se mantuvo intacto, demostrando que el estado interno del objeto está efectivamente protegido.

Ejecución en consola
<img width="1366" height="721" alt="{8A5ACB82-FB91-4588-8211-B7705F299A2E}" src="https://github.com/user-attachments/assets/bad5f46e-65ef-4a58-9a9e-994b307801c8" />

