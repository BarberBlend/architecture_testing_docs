# Arquitectura BarberBlend

Autor:
 - Jesus Andres Osorio


## 1 Introduccion

BarberBlend es una innovadora aplicación web diseñada para brindar una experiencia personalizada a los usuarios de Cali al elegir su barbería y estilista favorito en la ciudad. Con un enfoque intuitivo y fácil de usar, BarberBlend permite a los usuarios seleccionar sus preferencias, desde el tipo de servicio hasta el estilista de su elección, brindándoles un control total sobre su experiencia de cuidado personal.


## 2 Tecnologías y Herramientas Utilizadas

Lista de las tecnologías, lenguajes de programación, frameworks, plataformas y patrones de diseño utilizados en el proyecto:
- ### Backend 
- Lenguaje y framework: Java con Spring Boot
- Base de Datos: PostgreSQL en AWS RDS
- Autenticación: JWT (JSON Web Tokens) con Spring Security
- Envío de Correos Electrónicos: Gmail
- Patrones de diseño: DAO, DTO, Inyección de Dependencias, ORM.
- ### Frontend
- Lenguaje y framework: Next.js con TypeScript
- Framework CSS: TailwindCSS
- Patrones de diseño: Componentes reutilizables, renderización condicional.

Se seleccionaron estas tecnologías debido a su facilidad de uso, escalabilidad, y amplia comunidad de soporte. Spring Boot ofrece una configuración rápida y un ecosistema robusto para el desarrollo de aplicaciones Java. Next.js con TypeScript proporciona un desarrollo de frontend eficiente y tipado estático para una mejor calidad del código. PostgreSQL en AWS RDS ofrece escalabilidad y alta disponibilidad para la base de datos, mientras que Gmail se utiliza para el envío de correos electrónicos por su confiabilidad y facilidad de integración.

## 4 Atributos de Calidad

 Usabilidad:
- el aplicativo se va a basar en una interfaz de usuario intuitiva y facil de usar, teniendo un flujo claro para que el usuario pueda interactuar y navegar de manera sencilla 
- el aplicativo va a tener mecanismos de prevención de errores para los usarios, como comprobaciones de validación, mensajes de error, confirmaciones, alertas a los usuarios para que vuelvan a comprobar y corrijan los errores antes de que causen problemas.

 Rendimiento:
- la aplicacion va a ser capaz de responder solicitudes de manera rapida y eficiente, con un tiempo promedio de 5 segundos.

Seguridad
- La aplicacion protege al usario al momento de iniciar sesion, se genera un token al iniciar sesion con sus credenciales validas, el token es requerido para poder navegar en la aplicacion y tiene una duracion duracion de un mes.
- Al momento de registrarse la aplicacion va a encriptar la contraseña digitada mediante la libreria spreen security que usa Bcrypt para generar el hash 

Funcionalidad 
- la aplicacion permitira a los usuarios realizar tareas realcionadas con la busqueda y reserva de servicios de las barberias como:
Buscar barberias por nombre 
ver el perfil de cada barberia,incluyendo fotos, servicios y precios 
Reservar una cita en el dia y hora de su preferencia 
ver y cancelar citas 
recibir notificaciones via correo sobre el agendamiento de la cita 

## 5 Propuesta de implementación

Se presenta el modelado de la arquitectura mediante el modelo C4

![Model C4 Level2 (architecture of BarberBlend)](https://github.com/BarberBlend/architecture_testing_docs/blob/main/architecture-level2.png?raw=true)

## 6 Despligue
- El frontend se desplegará en un servicio de alojamiento estático como AWS S3, aprovechando la capacidad de almacenamiento escalable y la entrega de contenido a través de Amazon CloudFront para garantizar un rendimiento óptimo y una disponibilidad continua.
- El backend se implementará en AWS Elastic Beanstalk, un servicio administrado que simplifica el despliegue y la gestión de aplicaciones al manejar automáticamente tareas como el aprovisionamiento de recursos, el equilibrado de carga y la escalabilidad.

Para el despliegue se usara Github Actions para implementar prácticas de integración continua (CI) y entrega continua (CD).

