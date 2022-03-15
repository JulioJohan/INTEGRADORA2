# Integradora II
[![Contribuidores][contribuidores-shield]][contributors-url]

## contenido
<details>
  <summary>Tabla contenidos</summary>
  <ol>
    <li>
      <a href="#acerca-del-proyecto">Acerca del Proyecto</a>
      <ul>
        <li><a href="#descripción">Descripción</a></li>
        <li><a href="#objetivos">Objetivos</a></li>
        <li><a href="#organigrama">Organigrama</a></li>
        <li><a href="#diagrama-gantt">Diagrama Gantt</a></li>
      </ul>
    </li>
    <li>
      <a href="#análisis-de-la-solución">Análisis de la Solución</a>
      <ul>
        <li><a href="#requerimientos">Requerimientos</a></li>
        <li><a href="#diagrama-casos-de-uso">Diagrama de Casos de Uso</a></li>
      </ul>
    </li>
    <li>
      <a href="#diseño-de-la-solución">Diseño de la Solución</a>
      <ul>
        <li><a href="#modelo-relacional">Modelo Relacional</a></li>
        <li><a href="#diagrama-de-clases">Diagrama de Clases</a></li>
        <li><a href="#diagrama-de-componentes">Diagrama de Componentes</a></li>
      </ul>
    </li>    
    <li>
      <a href="#implementación">Implementación</a>
      <ul>
        <li><a href="#estándares-codificación">Estándares Codificación</a></li>
        <li><a href="#arquitectura">Arquitectura</a></li>
        <li><a href="#código-fuente">Código Fuente</a></li>
      </ul>
    </li>      
    <li>
      <a href="#pruebas">Pruebas</a>
      <ul>
        <li><a href="#casos-de-prueba">Casos de prueba</a></li>
        <li><a href="#ejecución">Ejecución</a></li>
      </ul>
    </li>       
    <li><a href="#guias">Guias</a></li>
    <li><a href="#contribucion">Contribución</a></li>
    <li><a href="#licencia">licencia</a></li>
    <li><a href="#contacto">Contacto</a></li>
    <li><a href="#participantes">Participantes</a></li>
  </ol>
</details>

<!-- Acerca del proyecto -->
## Acerca del proyecto
Requisitos.

<!-- Descripción -->
#### Descripción.
La idea es implementar una aplicación móvil híbrida y web que gestione la información correspondiente a tareas escolares mediante una base de datos. El funcionamiento del aplicativo es sencillo, ya que sólo consiste en un CRUD para agregar, eliminar o actualizar tareas mediante una interfaz intuitiva.

Por otro lado, el complemento de la aplicación es una pequeña lámpara que incluye un led RGB, esta permanece en color verde mientras no se han agregado tareas o se han terminado las tareas asignadas, cambia a color rojo cuando se agrega una nueva tarea y permanece en ese estado mientras haya tareas por realizar. Se pretende que la lámpara esté ubicada en un lugar visible, el escritorio por ejemplo, influyendo psicológicamente con el color rojo en la persona para que realice las tareas pendientes, y al terminarlas el color verde le hará sentir paz y tranquilidad ya que no habrá tareas pendientes. 
Tiempo: 5 horas semanales por desarrollador. 20 horas aproximadamente por semana (4 desarrolladores). 9 semanas aproximadamente.
Se estima un costo alrededor de $500.

<!-- Objetivos -->
#### Objetivos.
-Desarollar una aplicación móvil y web para facilitar la gestión de tareas.
-Apoyar al alumno con un mejor manejo de tareas y a equipos de trabajo que colaboran en un proyecto.

<!-- Organigrama -->
#### Organigrama.
Rol
Integrante
Líder: Mendoza Ramírez María Guadalupe 

Analista: Aguilar Castillo Karla Denisse

Diseñador: Guerrero Rodríguez Itzel Juliza

Programador: 
Aguilar Castillo Karla Denisse
Jaramillo Mejía Julio Johan
Mendoza Ramírez María Guadalupe.
Tester: Guerrero Rodríguez Itzel Juliza



<!-- Diagrama Gantt -->
#### Diagrama Gantt.
https://docs.google.com/spreadsheets/u/0/d/1dXE_BR3Gz3d_TjFGfFCTWc7TmBTwU3J8/edit 

<!-- Análisis del proyecto -->
## Análisis de la Solución.
En ésta sección se indicará los artefactos generados en base a la solución.

<!-- Requerimientos -->
#### Requerimientos.
Funcionales:

Número de requisito: RF01
Nombre de requisito: Registro de usuarios
Descripción: El aplicativo permite el registro de usuarios mediante suministro de datos: Nombre y Apellido, e-mail,usuario y contraseña.

Número de requisito: RF02
Nombre de requisito: Inicio de sesión
Descripción: El usuario podrá acceder al aplicativo mediante un inicio de sesión al ingresar el usuario y contraseña previamente registrados.

Número de requisito: RF03
Nombre de requisito:Gestión de tareas
Descripción: El usuario podrá realizar las siguientes acciones: agregar, consultar, modificar y eliminar tareas.
Cada tarea debe tener los siguientes datos:
  Id autogenerado por la aplicación.*
  Nombre de la tarea.*
  Descripción.*
  Fecha de entrega.*
  Estado (terminado o pendiente. En caso de marcar “terminado”, la tarea se eliminará.)*
  *Datos obligatorios.

No funcionales: 

Número de requisito: RNF01
Nombre de requisito: Especificación de registro
Descripción: El correo debe ser válido e irrepetible.
La contraseña debe contener un mínimo de seis caracteres sin restricciones.
Llenado de todos los campos solicitados.

Número de requisito: RNF02
Nombre de requisito: Recuperación de contraseña
Descripción: El aplicativo permite la restauración de la contraseña mediante el correo electrónico registrado por el usuario.

Número de requisito: RNF03
Nombre de requisito: Almacenamiento de información
Descripción: El aplicativo almacena la información en una base de datos MongoDB.

De comunicación:

Número de requisito: RDC01
Nombre de requisito: Comunicación con la lámpara
Descripción: La lámpara (arduino) tendrá comunicación con el servidor y la base de datos tendrá una reacción, si el usuario tiene proyectos (tareas) agregados la lámpara encenderá el led rojo y permanecerá hasta que el usuario no tenga tareas, cambiando el color a verde.


<!-- Diagrama de Casos de Uso -->
#### Diagrama Casos de Uso.
Agregar la imagen de los Casos de Uso.



<!-- Diseño del proyecto -->
## Diseño de la Solución.
![image](https://user-images.githubusercontent.com/90641538/158439236-6173c30b-73bd-4370-8743-2e94de35ebdc.png)


<!-- Modelo Relacional -->
#### Modelo Relacional.
Esquema de la base de datos (nombre de campo, tipo de datos, restricciones, etc)

<!-- Diagrama de Clases -->
#### Diagrama de Clases.
Esquema de las clases empleadas (atributos y sus métodos).

<!-- Diagrama de Componentes -->
#### Diagrama de Componentes.
Esquema de los componentes que interactúan (Modelo, Vista, Controlador, Servidor Web, Servidor de base de datos)


<!-- Implementación del proyecto -->
## Implementación.
En ésta sección se describe  los artefactos generados en base a la solución.

<!-- Estándares de Codificación -->
#### Estándares Codificación.
Estándares empleados en la codificación

<!-- Arquitectura MVC y Middleware -->
#### Arquitectura.
Definir los patrones empleados y de seguridad.

<!-- Código Fuente -->
#### Código Fuente.
Código Fuente de la solución


<!-- Pruebas proyecto -->
## Pruebas.
En ésta sección se describe  los artefactos generados en base a la solución.

<!-- Casos de prueba -->
#### Casos de prueba.
Indicar los casos de prueba

<!-- Ejecución Casos de prueba -->
#### Ejecución.
Evidencia de Ejecución de Casos de prueba.


<!-- Iniciando -->
## Iniciando
Iniciando.

<!-- Requisitos -->
### Requisitos
Requisitos de Instalación.

<!-- Instalación -->
### Instalacion
Instalación del Software


## Guias
Guias de Uso.

## contribucion
Contribucion.

## Licencia
Licencia.

## Contacto
Contacto.

## Participantes
* [participante 1]()
* [participante 2]()
* [participante 3]()

[contribuidores-shield]: https://img.shields.io/github/contributors/github_username/repo_name.svg?style=for-the-badge
[contributors-url]: https://github.com/github_username/repo_name/graphs/contributors
