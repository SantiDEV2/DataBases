# Celulares

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

### Relaciones

1. Un Cliente tiene un Pais (1-1)
2. Un Modelo tiene una Marca (1-1)
3. Un Modelo tiene unas Especificaciones (1-1)
4. Unas Especificaiones tienen varios Modelos (1-M)
5. Una Venta puede tener muchos Modelos (1-M)
6. Una Venta puede tener un Cliente (1-M)

### Tabla

<br>

![img](https://cdn.discordapp.com/attachments/948289759120351302/1035210763641565294/Diagrama_sin_titulo_1.jpg)

## Reglas de Negocio

- ### Clientes
1. Crear un cliente 
2. Leer todos los clientes
3. Leer un cliente en particular
4. Actualizar un cliente
5. Eliminar un cliente

- ### Marcas
1. Crear una Marca 
2. Leer todas las marcas
3. Leer una marca en particular
4. Actualizar una marca
5. Eliminar una marca

- ### Modelos
1. Crear un modelo
2. Leer todos los modelos
3. Leer un modelo en particular
4. Leer todos los modelos de una marca 
5. Actualizar un modelo
6. Eliminar un modelo

- ### Especificaciones
1. Crear unas especificaciones
2. Leer todas las especificaiones
3. Leer todos las especificaciones de un modelo
4. Actualizar unas especificaciones
5. Eliminar un articulo 

- ### Ventas 
1. Crear una venta
2. Leer todas las ventas
3. Leer una venta en particular
4. Leer todas las ventas de un cliente
5. Leer todas las ventas de un modelo
6. Actualizar una venta 
7. Eliminar una venta 

- ### Paises
1. Crear un pais
2. Leer todos los paises
3. Leer un pais en particular
4. Actualizar un pais
5. Eliminar un pais 