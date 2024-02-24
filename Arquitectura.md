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

## 3 Propuesta de implementación

Se presenta el modelado de la arquitectura mediante el modelo C4

![Model C4 Level2 (architecture of BarberBlend)](https://github.com/BarberBlend/architecture_testing_docs/blob/main/architecture-level2.png?raw=true)

## 4 Despligue
- El frontend se desplegará en un servicio de alojamiento estático como AWS S3, aprovechando la capacidad de almacenamiento escalable y la entrega de contenido a través de Amazon CloudFront para garantizar un rendimiento óptimo y una disponibilidad continua.
- El backend se implementará en AWS Elastic Beanstalk, un servicio administrado que simplifica el despliegue y la gestión de aplicaciones al manejar automáticamente tareas como el aprovisionamiento de recursos, el equilibrado de carga y la escalabilidad.

Para el despliegue se usara Github Actions para implementar prácticas de integración continua (CI) y entrega continua (CD).

