# MVC (modelo vista controlador)

## **¿Qué es el patrón MVC (Modelo Vista Controlador)?**

"MVC (Modelo-Vista-Controlador) es un patrón en el diseño de software comúnmente utilizado para implementar interfaces de usuario, datos y lógica de control. Enfatiza una separación entre la lógica de negocios y su visualización. Esta "separación de preocupaciones" proporciona una mejor división del trabajo y una mejora de mantenimiento."

**Para entender mejor el concepto de MVC vamos a definir cada uno de sus componentes:**

1. **Modelo:** Usualmente contiene lógica de negocio para leer y escribir información en la base de datos. Recibe peticiones del controlador y hace los cálculos, lecturas y escrituras necesarias para solventar la petición.
2. **Vista:** HTML que ve el usuario
3. **Controlador:** Código que se encarga de recibir peticiones del usuario, dirigirlos al modelo correspondiente y enviar la respuesta de regreso al usuario en caso de ser necesario

**En palabras más simples** , el patrón MVC nos permite separar la lógica de negocio en bloques de código independientes para poder reusarla en peticiones que la necesitan.