# Configuración de acceso anónimo

![](https://raw.githubusercontent.com/JosecarlosGlr/ConfiguracionDeAccesoAnonimo/refs/heads/main/1.png)

Para activar el acceso anónimo, he creado un usuario específico llamado **"anonymous"**. En el apartado de autenticación, he seleccionado la opción **"Do not require authentication"**, permitiendo así la conexión sin necesidad de contraseña.

![](https://raw.githubusercontent.com/JosecarlosGlr/ConfiguracionDeAccesoAnonimo/refs/heads/main/2.png)

Posteriormente, he configurado los puntos de montaje vinculando la ruta nativa `/home` al directorio raíz virtual `/`. Para cumplir con las directivas de seguridad, he establecido el modo de acceso en **"Read only"** (Solo lectura) y he desactivado la capacidad de escribir en la estructura de directorios.

![](https://raw.githubusercontent.com/JosecarlosGlr/ConfiguracionDeAccesoAnonimo/refs/heads/main/4.png)

Finalmente, he realizado la comprobación utilizando **FileZilla Client**. Como se observa en el log de la consola, la conexión TLS se establece correctamente y el usuario anónimo logra recuperar el listado del directorio sin errores, confirmando que el acceso restringido está operativo.
