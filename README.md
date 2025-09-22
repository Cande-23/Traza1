Proyecto en Java

Este proyecto implementa un modelo jerárquico usando Java orientado a objetos, aplicando encapsulamiento, multiplicidades y colecciones tipo HashSet para representar relaciones 1 a muchos. La clase App.java funciona como demo: instancia datos reales (ej.: Argentina → Buenos Aires/Mendoza → localidades → domicilios → sucursales → empresas) y permite realizar un CRUD básico sobre entidades de tipo Empresa.

Modelo y relaciones

Clases involucradas:
Pais, Provincia, Localidad, Domicilio, Sucursal, Empresa.

Relaciones modeladas:

Pais (1..n) → Provincia

Provincia (1..n) → Localidad

Localidad (1..n) → Domicilio

Sucursal (1–1) → Domicilio

Empresa (1..n) → Sucursal

Implementación técnica:

Uso de HashSet para manejar multiplicidades sin duplicados.

Métodos equals() y hashCode() definidos con cuidado para evitar ciclos o recursiones indeseadas.

Métodos toString() simplificados para facilitar la depuración.

Funcionalidades CRUD de Empresa:

Listar todas las empresas registradas

Buscar empresa por ID

Buscar empresa por nombre

Actualizar CUIT de empresa por ID

Eliminar empresa por ID

Requisitos técnicos:

Java 8 o superior

Lombok instalado y annotation processing activado en el IDE
