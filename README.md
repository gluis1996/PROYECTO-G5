## 2. Modelo De Negocio
En el Negocio a investigar consta de dos procesos una de ellas es la producción de prendas que se ejecuta en base a la oferta y a la demanda de los productos con el fin de mantener abastecido al punto de venta en este caso seria una tienda de Cercado de Lima, el segundo proceso consta en la venta de estos productos ya sea por unidad o por mayor con la finalidad de llevar una gestión correcta de las ventas y tener un análisis de los productos más demandados, ya que el vendedor puedo efectuar la veta al por mayor como por unidad. 

### 2.1.1 Modelo de Caso de Uso del Negocio

![MGCUN](ModeloGeneraldeCUN.png)


#### 2.1.1. Lista de los Actores del Negocio

|Nombre        |   Descripcion|
|-------------|-------------|
|Cliente|Trabajadores externos para la fabricación del producto|
|Proveedor|Agente externo que provee de material para la fabricación.|
|Contratistas|Agente Externo que solicita los productos|

#### 2.1.2. Lista de Casos de Uso del Negocio

|Nombre        |   Descripcion|
|-------------|-------------|
|Gestión de Pedido|Área en la que se ingresa el pedidoo|
|Gestión de Requerimiento de material|Área en la que verifica el material si no la hay suficiente se procede a solicitarlo|
|Gestión de abastecimiento|Área que se encarga de abastecer con material al negocio|
|Gestión de Fabricación|Área que se encargar del corte y la distribución a las service|
|Gestión de Entrega|Área que se encarga de entregar los pedidos al cliente|

#### 2.1.3. Diagrama de Casos de Uso del Negocio

![DCUN](DiagramaGeneralMCUN.png)

#### 2.1.4. Especificaciones de Casos de uso del Negocio
##### ECU Gestion de Pedido
###### Especificaiones de Alto Nivel
|Nombre        |   Gestión de Pedido|
|-------------|-------------|
|Descripción|Este proceso comienza cuando con el cliente solicitando una cierta cantidad de prendas, si la cantidad de prendas solicitada está dentro del stock de la tienda se procede con la venta en caso contrario se procede a realizar una orden de pedido con un plazo mínimo de días para la entrega.|
|Actores de negocio|Vendedor, Cliente|
|Entradas|Ingreso de solicitud de pedido|
|Entregables|Entrega del pedido del cliente|
|Mejoras |Satisfacer la Necesidades de los clientes|

###### Especificación de detalle nivel

|NOMBRE DEL CASO DE USO        |   Gestión de Pedido|
|-------------|-------------|
|ACTOR |Vendedor, Cliente|
|OBJETIVO|Satisfacer la Necesidades de los clientes|
|BREVE DESCRIPCION|Este proceso tiene como finalidad aumentar las ventas y fidelizar a los clientes|
|PRECONDICIONES|-La venta debe de ser mayor a 100 prendas -El requerimiento mínimo debe de ser 50 prendas-Se debe efectuar el pago total por la cantidad del stock en tienda + un 10% de lo faltante|
|FLUJO BASICO DE EVENTOS |    1. El vendedor recibe el requerimiento del cliente     2. El vendedor ingresa los datos del cliente     3. El vendedor informa sobre los plazos de entrega     4. El vendedor registra el pedido del cliente 5. Fin del proceso|
|FLUJO ALTERNO|1. El vendedor verifica el stock en tienda. 1.1 Si hay stock en tienda se va al paso 3 2. El vendedor disuade al cliente con otros modelos en caso no haya en tienda 2.1 Si el cliente no acepta se va al paso 3 3. Si el vendedor no está conforme con los plazos de entrega se va al paso 5|
|POSTCONDICIONES|Se le entrega una boleta de pedido.|

###### DA Gestion de Pedido
![DA-GP](DA_GestiondePedido.png)

##### ECU Gestión de Entrega
###### Especificaiones de Alto Nivel
|Nombre        |   Gestión de Pedido|
|-------------|-------------|
|Descripción|Este proceso se realiza cuando el pedido del cliente haya terminado la gestión de abastecimiento, por siguiente se busca el producto solicitado para ser empaquetado y finalmente entregado al cliente.|
|Actores de negocio|Despachador, Cliente|
|Entradas|Ingreso de solicitud de entrega|
|Entregables|Entrega del pedido del cliente|
|Mejoras |Satisfacer la Necesidades de los clientes|

###### Especificación de detalle nivel

|NOMBRE DEL CASO DE USO        |   Gestión de Entrega|
|-------------|-------------|
|ACTOR |Despachador, Cliente|
|OBJETIVO|Satisfacer la Necesidades de los clientes|
|BREVE DESCRIPCION|Este proceso tiene como finalidad aumentar las ventas y fidelizar a los clientes|
|PRECONDICIONES|-La venta debe de ser mayor a 100 prendas -El requerimiento mínimo debe de ser 50 prendas-Se debe efectuar el pago total por la cantidad del stock en tienda + un 10% de lo faltante|
|FLUJO BASICO DE EVENTOS |    1.  El despachador recibe la solicitud de entrega     2. El despachador ubica el pedido     3. El despachador empaca el producto final     4. El despachador registra la salida del producto 5. El despachador entrega el producto al cliente 6.  Fin del proceso|
|FLUJO ALTERNO||
|POSTCONDICIONES|Se le entrega una boleta de pedido.|