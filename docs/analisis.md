# Análisis – Sistema de gestión de gimnasio

## Problema
El gimnasio registra socios, pagos y asistencias a mano. No sabe rápido quién debe la cuota, los datos se pierden y no se pueden pasar a otras herramientas.

## Alcance
Programa de consola en Java usado por **un solo actor: el recepcionista**. No incluye login ni roles (queda fuera del alcance porque no aporta al tema de la clase).

## Requerimientos funcionales
| N° | Requerimiento | Archivo |
|----|---------------|---------|
| RF1 | Dar de alta un socio (DNI, nombre, apellido, teléfono, plan) | socios.csv |
| RF2 | Dar de baja un socio por DNI | socios.csv |
| RF3 | Buscar un socio por DNI | socios.csv |
| RF4 | Listar todos los socios | socios.csv |
| RF5 | Registrar el pago de una cuota y actualizar su vencimiento | pagos.csv |
| RF6 | Registrar el ingreso de un socio al gimnasio | asistencias.txt |
| RF7 | Ver las asistencias de un socio | asistencias.txt |
| RF8 | Importar socios desde un CSV externo | archivo elegido |
| RF9 | Exportar a CSV los socios con cuota vencida | morosos.csv |
| RF10 | Cargar los datos al iniciar y guardarlos al salir | socios.csv, pagos.csv |

## Requerimientos no funcionales
- Los datos se guardan en archivos dentro de la carpeta `datos/` del proyecto.
- Los CSV se leen y escriben con la librería **opencsv** (proyecto Maven).
- El programa no debe cerrarse por un error: todos los errores de archivos y de datos se informan con un mensaje claro.

## Reglas del negocio y validaciones
- No puede haber dos socios con el mismo DNI.
- El monto de un pago debe ser mayor a 0.
- No se puede registrar un pago ni un ingreso de un DNI que no existe.
- Si un archivo no existe al iniciar, se crea vacío.
- Si una línea de un CSV está mal formada, se saltea y se informa, sin cortar la carga.

## Historias de usuario
1. Como recepcionista, quiero dar de alta un socio para tenerlo registrado.
2. Como recepcionista, quiero buscar un socio por DNI para ver sus datos y si debe la cuota.
3. Como recepcionista, quiero registrar un pago para que el socio quede al día.
4. Como recepcionista, quiero anotar cada ingreso para saber cuánto viene cada socio.
5. Como dueño, quiero exportar la lista de morosos para avisarles que deben la cuota.
6. Como dueño, quiero importar mi lista vieja de socios desde Excel (CSV) para no cargarlos de nuevo a mano.
7. Como recepcionista, quiero que los datos sigan ahí cuando vuelvo a abrir el programa.
