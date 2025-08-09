# Propuesta TP DSW

## Grupo
### Integrantes
* 49822 - Sesana, Octavio
* 50029 - Di Marco, Martin
* 49373 - Salvía, Camila
* 50026 - Vivas, Martin Ariel

### Repositorios
* frontend: https://github.com/camila-salvia/frontend-tp-dws2024
* backend: https://github.com/OctavioSesana/backend

## Tema
### Descripción
Sistema de alquiler de canchas de fútbol de dos tipos: Fútbol 5 y Fútbol 7.

### Modelo

Link Drive: https://drive.google.com/drive/folders/1Spls67U-GuqDTieQFtbJXADwzbpLSfh7


## Alcance Funcional 

### Alcance Mínimo
PROXIMA ENTREGA: se realizará la CRUD Cliente

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Tipo Cancha<br>2. CRUD Cliente<br>3. CRUD Reserva|
|CRUD dependiente|1. CRUD Cancha {depende de} CRUD Tipo Cancha<br>2. CRUD Reserva {depende de} CRUD Tipo de cancha|
|Listado<br>+<br>detalle| 1. Listado de canchas disponibles filtrado por tipo de cancha, muestra código y tipo => detalle CRUD Canchas<br> 2. Listado de reservas para el usuario correspondiente (muestra mail del mismo), muestra código de cancha, fecha, y hora de inicio. => detalle muestra datos completos de la reserva y mail del cliente con la sesión iniciada|
|CUU/Epic|1. Reservar una cancha para jugar<br>2. Cobrar alquiler de cancha|

## Testings
### Backend
#### Test Unitario - Módulo de Reservas
Para asegurar la calidad del código, se implementó un test unitario en el backend para validar el formato de hora de las reservas. Este test verifica que una función de utilidad reciba correctamente la hora en formato HH:mm (ej. "19:00"), lo cual es crucial para la consistencia de los datos en la base de datos.

El test se ejecutó usando el framework Jest y el resultado fue el siguiente:
<img width="625" height="238" alt="image" src="https://github.com/user-attachments/assets/18c65543-96a3-4d5b-96b2-69a463650b40" />
Este resultado confirma que la función de validación de hora opera según lo esperado, garantizando la integridad del formato de datos en una parte crítica de la aplicación.

