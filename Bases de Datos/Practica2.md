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

