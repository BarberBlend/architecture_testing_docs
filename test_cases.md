# Casos de prueba

## Caso de prueba 1: Acceso a la lista de barberías desde la página principal de BarberBlend:

### Precondición: El usuario ha iniciado sesión en la aplicación BarberBlend.

#### Pasos:
- Ingresar a la página principal de BarberBlend.
- Buscar y hacer clic en la opción "Lista de Barberías".

#### Resultado esperado: 
El usuario debe ser redirigido a la página que muestra la lista completa de barberías disponibles.




## Caso de prueba 2: Reserva de cita para corte de cabello en una barbería específica:

### Precondición: El usuario ha iniciado sesión en BarberBlend y se encuentra en la página de una barbería.

#### Pasos:
- Seleccionar la barbería de preferencia.
- Elegir el servicio de "Corte de Cabello".
- Explorar los estilistas disponibles y elegir uno.
- Seleccionar la fecha y hora deseada para la cita.
- Confirmar la reserva.

#### Resultado esperado: 
El usuario debería recibir una notificación de que la cita para el corte de cabello ha sido agen



## Caso de prueba 3: Búsqueda avanzada de barberías por nombre:

### Precondición: El usuario ha iniciado sesión en BarberBlend y se encuentra en la página principal.

#### Pasos:
- Utilizar la barra de búsqueda.
- Ingresar el nombre de una barbería específica.
- Hacer clic en la opción de búsqueda.

#### Resultado esperado:
Deberían mostrarse resultados que incluyan la barbería cuyo nombre se ingresó en la barra de búsqueda.

## Caso de prueba 4: Intento de reserva fuera del horario de trabajo:

### Precondición: El usuario ha iniciado sesión y está en la página de reserva de citas.

#### Pasos:
- Seleccionar un estilista.
- Intentar reservar una cita en un horario no disponible según la agenda del estilista.
- Confirmar la reserva.

#### Resultado esperado: 
El sistema debería mostrar un mensaje indicando que el estilista no está disponible en el horario seleccionado y sugerir alternativas



## Caso de prueba 5: Exploración de detalles de una barbería desde la lista:

### Precondición: El usuario ha iniciado sesión y se encuentra en la lista de barberías.

#### Pasos:
- Seleccionar una barbería de la lista.
- Explorar la información detallada de la barbería, como servicios ofrecidos y ubicación.

#### Resultado esperado: 
El usuario debería poder acceder y explorar los detalles de una barbería específica desde la lista.
