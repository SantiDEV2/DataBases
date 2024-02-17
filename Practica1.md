# Celulares

## Explicacion
Un modelo de base de datos para la compra de celulares, esta consiste en las tablas que tendriamos asi como las llaves principales y las llaves foraneas

### Clientes 
- ID_Clientes (**__PK__**)
- Nombre
- Apellidos
- Telefono
- Email
- Direccion 
- CP
- Ciudad
- Pais (**__FK__**)

### Marcas 
- ID_Marca (**__PK__**)
- Nombre de Marca 
- Sistema Operativo
- Fecha de Fundacion
- Lugar de Fundacion 
- Fundadores  

### Modelos
- ID_Modelos (**__PK__**)
- ID_Marca (**__FK__**)
- Nombre de Modelo
- Año de lanzamiento
- ID_Especificaciones (**__FK__**)

### Especificaciones
- ID_Especificaciones (**__PK__**)
- ID_Modelos (**__FK__**)
- Pantalla
- Camara Principal
- Memoria 
- Procesador 
- Precio 

### Ventas
- ID_Ventas (**__PK__**)
- ID_Modelo (**__FK__**)
- ID_Cliente (**__FK__**)

### Paises
- ID_Paises (**__PK__**)
- Nombre
- Dominio