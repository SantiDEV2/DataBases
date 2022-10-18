# Celulares

### Marcas 
- ID_Marca (**__PK__**)
- Sistema Operativo
- Nombre de Marca 
- Fecha de Fundacion
- Lugar de Fundacion 
- Fundadores  

### Modelos
- ID_Modelos (**__PK__**)
- Nombre de Modelo
- Año de lanzamiento
- ID_Especificaciones (**__FK__**)


### Especificaciones
- ID_Especificaciones (**__PK__**)
- ID_Modelos (**__FK__**)
- Pantalla
- Camara
- Memoria 
- Procesador 
- Precio 

### Ventas
- ID_Ventas (**__PK__**)
- ID_Marca (**__FK__**)
- Numero de Ventas
- Lugar de Fabricación 
