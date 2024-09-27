# Proyectos

## Microsoft Teams

Cada PROYECTO tiene su equipo de Teams -> Poder usar Microsoft Planner y mantener archivos ocultos.

Para el PROYECTO en cuestión se creará el equipo privado: CCMSS-PROYECTO.

Para cada paquete de trabajo se creará un CANAL dentro del equipo y se sincronizará la carpeta de archivos en el One Drive local del usuario. La estructura de directorios deberá quedar como se muestra a continuación:

    CCMSS-PROYECTO (equipo de MS Teams)
      └── CANAL (carpeta de MS Teams sincronizada)

## GitHub

Después se ha de crear un repositorio de código para el proyecto, el repositorio se llamará PROYECTO
  - Los canales (subdivisiones del proyecto) serán submódulos de ese mismo repositorio.
  - Para el CANAL, el repositorio creado habrá de llamarse: PROYECTO-CANAL.
  - Para añadir el submódulo al proyecto se utilizará el siguiente comando de git dentro del directorio del propio proyecto:

          git submodule add https://github.com/ccmss-upm/XXX-YYY
    
  - Después, se añadirá al submódulo local la carpeta sincronizada con MS Teams para conseguir la siguiente esturctura de directorios:

        PROYECTO (repositorio de github)
          └── PROYECTO-CANAL (submódulo del repositorio)
            └── CANAL (carpeta de MS Teams sincronizada)

  - Ejemplo de estructura:
        
        AIRE (repositorio de github)
          └── AIRE-E1 (submódulo del repositorio)
            └── E1 (carpeta de MS Teams sincronizada)
              ├── E1-1
              │ └── Deliverable
              │    └── References
              ├── E1-2
              │ ├── Datos Ensayo
              │ └── Report
              |    └── Notas Tomadas Durante Ensayo
              ├── E1-3
              │ ├── Propuesta
              │ └── Shoppings
              └── Reports
                ├── 0_Informe Original
                └── 99_Documentación



# Herramientas

Cuando se desarrollen herramientas de software se crearán dos repositorios: uno PRIVADO que contendrá el código y las instrucciones de uso y uno PÚBLICO que contendrá información sobre el proyecto que pueda ser mostrada.

Si la herramienta es desarrollada de forma individual se agragará como colaboradora a esta cuenta para que se pueda realizar un FORK SIN COPIAR para tenerla así sincronizada con el estado último del repositorio
