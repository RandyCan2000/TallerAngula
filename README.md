## Angular

Instalacion de Angular cli

### Pre-Requisito
- Tener Instalado [nodejs][key]

[key]: https://nodejs.org/es/

### Instalacion 

    Abrir Terminal y copiar el siguiente comando
    > npm install -g @angular/cli


### Iniciar Nuevo Proyecto

    Paso 1 
    Abrir una Terminal

    Paso 2
    Escribir el siguiente comando:
    > ng new NombreProyecto --routing
        Ejemplo
        ng new ProyectoIntermedias --routing
    
    Paso 3 
    Entrar a la carpeta de nuestro proyecto
    > cd NombreProyecto
        Ejemplo
        cd ProyectoIntermedias
    
    Paso 4
    copiar el siguiente comando
    > ng server
        Esto levantara el proyecto de angular en el puerto 4200

    Si se desea cambiar de puerto se debe ejecutar el siguiente comando
    > ng server --port puerto
        Ejemplo
        ng server --port 3000

### Generar Componentes
- Navegar hasta la carpeta app por medio de la terminal.

     * crear una carpeta para guardar los componentes
     * Ingresar a esta carpeta nueva
     * Ejecutar el comando:

                > ng generate component Nombre_Componente

            abreviatura

                > ng g c Nombre_Componente

            Ejemplo

                > ng generate component Home
                > ng g c Home

### Generar Servicios
- Navegar hasta la carpeta app por medio de la terminal.

     * crear una carpeta para guardar los Servicios
     * Ingresar a esta carpeta nueva
     * Ejecutar el comando:

                > ng generate service Nombre_Servicio

            abreviatura

                > ng g S Nombre_Servicio

            Ejemplo

                > ng generate service Song_Services
                > ng g s Song_Services

### Angular Material

    Ejecutar en la terminal de nuestro proyecto
    > ng add @angular/material

- Copiar la Carpeta material en la carpeta app del proyecto
- Ir al archivo app.module.ts e importar la clase dentro de la carpeta material de la siguiente forma

        import { MaterialModule } from './material/material.module';
- En @NgModule en el arreglo imports escribir MaterialModule

        imports: [
            BrowserModule,
            AppRoutingModule,
            BrowserAnimationsModule,
            MaterialModule //<-- de esta forma              
            ],


# Proyecto de Ejemplo

- Repositorio de Ejemplo completo utilizando angular como frontend, Django para backend [SongApp][key2]

[key2]: https://github.com/carlosngv/SongApp