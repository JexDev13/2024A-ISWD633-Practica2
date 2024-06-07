# Variables de Entorno
### ¿Qué son las variables de entorno
# COMPLETAR

### Para crear un contenedor con variables de entorno

```
docker run -d --name <nombre contenedor> -e <nombre variable1>=<valor1> -e <nombre variable2>=<valor2>
```

### Crear un contenedor a partir de la imagen de nginx:alpine con las siguientes variables de entorno: username y role. Para la variable de entorno rol asignar el valor admin.

# COMPLETAR

# CAPTURA CON LA COMPROBACIÓN DE LA CREACIÓN DE LAS VARIABLES DE ENTORNO DEL CONTENEDOR ANTERIOR

![image](https://github.com/JexDev13/2024A-ISWD633-Practica2/assets/119013519/19fba6df-d71b-4ed3-a787-1a8c7f76c164)


### Crear un contenedor con mysql:8 , mapear todos los puertos
# COMPLETAR

![image](https://github.com/JexDev13/2024A-ISWD633-Practica2/assets/119013519/749b0e1a-0c2d-454e-80b4-bcee84b355c6)




### ¿El contenedor se está ejecutando?
# COMPLETAR
No esta ejecutando
![image](https://github.com/JexDev13/2024A-ISWD633-Practica2/assets/119013519/62b02ce6-a035-4253-93fd-39a1f09ac6d7)




### Identificar el problema
# COMPLETAR
Falta las variables de entorno
![image](https://github.com/JexDev13/2024A-ISWD633-Practica2/assets/119013519/02bae363-f222-48fe-87d9-e35e5df436b0)

### Eliminar el contenedor creado con mysql:8 
# COMPLETAR
![image](https://github.com/JexDev13/2024A-ISWD633-Practica2/assets/119013519/5aa1aa51-ab84-46c9-bb37-fe3105de05c6)


### Para crear un contenedor con variables de entorno especificadas
- Portabilidad: Las aplicaciones se vuelven más portátiles y pueden ser desplegadas en diferentes entornos (desarrollo, pruebas, producción) simplemente cambiando el archivo de variables de entorno.
- Centralización: Todas las configuraciones importantes se centralizan en un solo lugar, lo que facilita la gestión y auditoría de las configuraciones.
- Consistencia: Asegura que todos los miembros del equipo de desarrollo o los entornos de despliegue utilicen las mismas configuraciones.
- Evitar Exposición en el Código: Mantener variables sensibles como contraseñas, claves API, y tokens fuera del código fuente reduce el riesgo de exposición accidental a través del control de versiones.
- Control de Acceso: Los archivos de variables de entorno pueden ser gestionados con permisos específicos, limitando quién puede ver o modificar la configuración sensible.

Previo a esto es necesario crear el archivo y colocar las variables en un archivo, **.env** se ha convertido en una convención estándar, pero también es posible usar cualquier extensión como **.txt**.
```
docker run -d --name <nombre contenedor> --env-file=<nombreArchivo>.<extensión> <nombre imagen>
```
**Considerar**
Es necesario especificar la ruta absoluta del archivo si este se encuentra en una ubicación diferente a la que estás ejecutando el comando docker run.

### Crear un contenedor con mysql:8 , mapear todos los puertos y configurar las variables de entorno mediante un archivo
# COMPLETAR
![image](https://github.com/JexDev13/2024A-ISWD633-Practica2/assets/119013519/0b933718-3fc4-4834-b60d-14466ea79820)



# CAPTURA CON LA COMPROBACIÓN DE LA CREACIÓN DE LAS VARIABLES DE ENTORNO DEL CONTENEDOR ANTERIOR 
![image](https://github.com/JexDev13/2024A-ISWD633-Practica2/assets/119013519/9bcd2075-d565-4bbb-979e-591438544326)


### ¿Qué bases de datos existen en el contenedor creado?
# COMPLETAR
![image](https://github.com/JexDev13/2024A-ISWD633-Practica2/assets/119013519/6eed790f-9cf0-4d6d-b718-0f4e50e7186c)
