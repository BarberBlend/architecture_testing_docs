# Arquitectura para el modulo barber 

Autor:
 - Jesus Andres Osorio


## 1 TL;DR

Se crean varios componentes para listar barberias y ver la informacion de la barberia. Estos componentes realizar las siguientes funciones:

- Listar todas las barberias disponibles
- Buscar una barberia por nombre
- Ver la informacion de la barberia seleccionada


## 2 Motivación

Como una aplicación web innovadora llamada BarberBlend, nuestro objetivo es proporcionar a los usuarios de Cali una experiencia única al seleccionar su barbería y barbero preferido en la ciudad. Con un enfoque intuitivo y accesible, los usuarios pueden personalizar su experiencia eligiendo entre una variedad de servicios, incluyendo cortes de cabello, arreglos de barba o ambos, y seleccionando al estilista de su elección. En BarberBlend, ponemos el control en manos de nuestros usuarios, brindándoles una experiencia de cuidado personal sin igual en la vibrante ciudad de Cali.

## 3 Propuesta de implementación

Se propone unos componentes que contenga la logica requerida para obtener la informacion necesario y mostrarla mediante endpoints.

![Model C4 Level3 (architecture of BarberBlend)](https://github.com/BarberBlend/architecture_testing_docs/blob/main/architecture-level3.png?raw=true)


### 3.1 Service - Backend-Service-Barbers

Este servicio devuelve el listado de las barberias disponibles en Cali, ademas de que tambien traer la informacion de una barberia en especifico mediante un parametro que se le pasara al servicio en el EndPoint, con el formato de babers/{id}, de esta manera obteniendo el contenido de la base de datos tanto para una barberia en especifico o un listados de las barberias disponibles.

## 4 Tecnologías

- Java como lenguaje en el servicio
- Se usara PostgreSQL como motor de base de datos
