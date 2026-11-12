# grupo1-emprendimiento-digital.
Sistema de gestión de socios para un gimnasio – AED2, Clase 10: Archivos de texto y CSV
# Gimnasio - Sistema de Gestión de socios

**Materia:** Algoritmos y estructuras de datos 2 (AED2), Prof. Silvina Burgos 
**Integrantes**
- Diego ALtamirano : GitHUb : "Usuario"
- Mateo Aramayo : GitHub :"Usuario"
- Pires Alan Joel : GitHub : @pires12334

**Tablero kanban:** https://trello.com/b/ErUSUj3k/por-hacer

## Descripción del negocio 
Gimnasio de barrio con planes mensuales (musculacion, funcional, pase libre). Sus clientes son socios que pagan una cuota por mes y asisten varias veces por semana.

##Problema que resuelve
Hoy el gimnasio anota socios, pagos e ingresos en un cuaderno o en plantillas sueltas. No sabe rapido quien tiene la cuenta vencida, los datos se pierden o se duplican y no hay un registro confiable de asistencias.

El programa guarda toda la informacion en **archivos** (CSV y texto) para que los datos no se pierdan al cerrar el sistema y se puedan importar y exoportar.

##Tema elegido
**clase 10: Archivos de texto y CSV**
Lo elegimos porque el problema principal del negocio es *guardar y recuperar informacion*: un gimnasio necwesita conservar los datos de sus socios entre un dia y el otro, y poder pasarlos a otras herramientas (por ejemplo, Excel) en formato CSV
(Nota: al principio del proyecto habiamos elegido la clase 8 con una clinica. El 11/11 cambiamos a la clase 10 con un gimnasio.)

## Tecnologias 
- Java 17
- Maven
- opencsv (lectura y escritura de CSV)
- java.io (FileWriter, FileReader, BufferedReader)

## Cómo ejecutar el proyecto
1. Clonar el repositorio.
2. *(Se completa en el Día 4–5)*

## Funcionalidades
- Alta, baja, búsqueda y listado de socios (socios.csv)
- Registro de pagos de cuota (pagos.csv)
- Registro de ingresos al gimnasio (asistencias.txt)
- Importar socios desde un CSV externo
- Exportar socios con cuota vencida (morosos) a CSV
- Manejo de errores: archivo inexistente, línea mal formada, DNI duplicado, datos inválidos

## Capturas de pantalla
*(Se completa al final)*

## Pruebas realizadas
*(Ver carpeta /pruebas)*

## Conclusiones
*(Se completa al final)*
