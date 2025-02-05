---
layout: default
title: Pedidos
permalink: /Operacion/scm/ventas/vpedido/vped
editable: si
---

# Pedidos - VPED


Esta aplicación contiene una pantalla maestra que sirve para adicionar, consultar y modificar los pedidos que hacen los clientes a la empresa.


>+ [**Consultas dinámicas**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#consultas-dinámicas)
>+ [**Verificación de Pedidos**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#verificación-de-pedidos)
>+ [**Itemchanged campos Precio y Porcentaje de Descuento**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#itemchanged-campos-precio-y-porcentaje-de-descuento)
>+ [**Botón Info Ventas**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#botón-info-ventas)
>+ [**Ver Saldo Por Ubicación**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#ver-saldo-por-ubicación)    
>+ [**Cómo relacionar un pedido a una cotización**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#cómo-relacionar-un-pedido-a-una-cotización)  
>+ [**Cómo relacionar un pedido a una factura**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#cómo-relacionar-un-pedido-a-una-factura)  
>+ [**Pedidos con separada**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#pedidos-con-separada)  
>+ [**Monto mínimo en un pedido**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#monto-mínimo-en-un-pedido)  
>+ [**Actualizar Datos de Cliente**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#actualizar-datos-de-cliente)   

---
Esta pantalla es fundamental para la captura de las órdenes de compra de los clientes ya que se encuentra integrada a los módulos de cartera e inventarios, con cartera en la validación del cupo y condiciones comerciales y con inventarios en la disponibilidad de los productos.  


![](vped1.png)


**Documento:** PD de pedido.  
**Número:** consecutivo generado automáticamente.  
**Ubicación:** Número de ubicación de la empresa la cual realiza el documento.  
**Concepto:** PD de pedido.  
**Motivo:** Motivo parametrizado previamente en la aplicación **BMOT**.  
**Fecha:** Fecha en que se registra el pedido.  
**Tercero:** Número de identificación del tercero que solicita el pedido. Con clic derecho permite crear clientes abre un nuevo formulario:  
![](vped51.png)  
![](vped52.png)  

**Nombre Tercero:** Nombre del tercero que solicita el pedido.  


![](vped2.png)

**Moneda:** Doble clic y seleccionar tipo de moneda utilizada para el pedido.  
**Estado:** Estado del pedido: Activo, Procesado, Anulado.  
**Vendedor:** Número de cédula del vendedor.  
**TipoPrecio:** Doble clic y seleccionar si es Normal y Minoristas.  
**% Descuento:** Número del porcentaje de descuento a realizar.  
**Ordencompra:** Número de la orden de compra.  
**Condición Pago:** Doble clic y seleccionar la condición de pago acordada.  

![](vped3.png)

**Bruto:** Valor bruto del pedido.  
**Descuento:** Valor en cifras del descuento acordado.  
**Subtotal:** Resta del valor bruto menos el descuento acordado.  
**TaxSale:** Valor de impuestos.  
**Total:** Suma del subtotal más el valor de los impuestos.  
**Impreso:** Se marca cuando se ha impreso el documento.  
**DeliveryDateMax:** Fecha de entrega máxima.  

![](vped4.png)

**Crédito:** Estado del crédito.  
**Comercial:** Estado de aprobación por comercial.  
**Liberación:** Si se liberó o no.  
**LiberationCommercial:** Si la liberación se realizó por comercial.  
**Consignación:** Si se realizó la consignación o no.  
**ProjectId:** Identificación del proyecto al que pertenece.  
**Observación:** Comentarios.  
***************
Esta aplicación consta de una ventana en la parte inferior llamada detalle:

![](vped5.png)

**Renglón:** Número del renglón del detalle a registrar.  
**Producto:** doble clic y seleccionar número del producto.  
**Nombre Producto:** Nombre del producto arrojado automáticamente.  
**Cantidad:** Cantidad del producto del pedido.  
**Precio:** Precio del producto.  
**%Imp:** Número del porcentaje de impuesto.  
**%Descuento:** Número del porcentaje de descuento del pedido.  


![](vped6.png)

**Total:** Valor total del pedido.  
**Bodega:** Bodega de donde proviene el producto.  
**Fecha Entrega:** Fecha de entrega del pedido.  
**Control:** Permite controlar el inventario por un número de control, es decir, como un identificador.  

************
![](vped21.png)

**Localización:** Identificación numérica de la localización de un producto.  
**Característica:** Código de la característica que se puede atribuir al producto.  
**Presentación:** Forma de presentación del producto.  
**Vencimiento:** Fecha de vencimiento del producto.  
**Control:**  Número de serial o consecutivo asignado a productos que vende la empresa y 	poder así identificarlos y llevar un control sobre ellos.  
**Id Lote:** Si los productos pertenecen a un lote en específico.  
**Estado:**  activo, procesado o anulado.  
**Unidad Medida:** parametrización del BMED.   
**Observación:** campo a editar o comentar.  
**Código Antiguo:** referencia código del producto.  


## [Consultas dinámicas](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#consultas-dinámicas)

Realización de una consulta dinámica en la aplicación _VPED - Pedidos_.  

![](vped7.png)

## [Verificación de Pedidos](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#verificación-de-pedidos)

Realizado el pedido en la aplicación [**Comprar**](http://docs.oasiscom.com/Operacion/marketplace/comprar), ingresaremos a la aplicación _VPED - Pedidos_ y filtraremos por la fecha en la que se realizó nuestro pedido. Si los productos y/o servicios seleccionados corresponden a diferentes proveedores, se generarán dos transacciones diferentes en VPED.  

En el ejemplo del pedido realizado en la aplicación [**Comprar**](http://docs.oasiscom.com/Operacion/marketplace/comprar), seleccionados una jarra y una maleta, estos dos artículos son de proveedores diferentes, por lo tanto se verán los pedidos en dos documentos diferentes como se muestra a continuación.  

Pedido de la Jarra

![](vped8.png)

Pedido de la Maleta

![](vped9.png)


## [Itemchanged campos Precio y Porcentaje de Descuento](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#itemchanged-campos-precio-y-porcentaje-de-descuento)


El objetivo del itemchanged en el campo _Precio_ y _Porcentaje Descuento_, es que el sistema valide que al final el precio que coloque el usuario no esté por debajo del valor de referencia de la lista de precios. Este precio de referencia estará definido  en la aplicación FPRE en el campo _Valor1_.  

En la aplicación [**FBTP - Tipo de Precio**](http://docs.oasiscom.com/Operacion/scm/facturacion/fbasica/fbtp) debemos asignar al tipo de precio la característica _Variable_.  

![](fbtp.png)

En la aplicación [**FPRE - Precios**](http://docs.oasiscom.com/Operacion/scm/facturacion/fprecio/fpre) se definirá el precio.  

![](fpre.png)

Con el nuevo precio y descuento asignado, el sistema deberá mostrar un mensaje de alerta y no se deberá poder salvar los cambios.  


En VPED intentamos ingresar un precio y un descuento.  

![](vped10.png)

Al intentar ingresar el precio de 390 y dar tab, el sistema muestra el mensaje de control, puesto que, quedaría un precio de 360 cual está por debajo de los 380 de la lista de precios. Lo mismo debe pasar si se asigna en % de descuento que haga que el precio quede por debajo del rango mínimo.  

![](vped11.png)

Si se trata de guardar la información sin dar tab, el sistema debe mostrar el mensaje de control.  

![](vped12.png)


## [**Botón Info Ventas**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#botón-info-ventas)

Este botón permite visualizar la fecha de la última compra del producto así como el precio con el que fue vendido.  

El botón **info_ventas** en el detalle de la opción _VPED_, permite visualizar la fecha de la última compra del producto así como el precio con el que fue vendido.  

![](vped13.png)

![](vped14.png)

## [**Ver Saldo Por Ubicación**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#ver-saldo-por-ubicación)

Esta función permite ver el saldo por ubicación del detalle de un producto en especifico.

Para ver esta información se debe dar clic derecho sobre el detalle del producto que deseamos ver y seleccionamos "**Ver saldo por Ubicacion**"

![](vped53.png)

Se visualiza la siguiente ventana:

![](vped55.png)

* Botón **Agregar y Continuar**, para reanudar la inserción de documentos.  
* Botón **Aceptar** para insertar los ítems seleccionados y cierra el zoom de búsqueda. 


##  [**Cómo relacionar un pedido a una cotización**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#cómo-relacionar-un-pedido-a-una-cotización)  

Para conocer el proceso completo, por favor diríjase a: [Cómo relacionar un pedido a una cotización](http://docs.oasiscom.com/Operacion/scm/ventas/vcotizacio/vcot#cómo-relacionar-un-pedido-a-una-cotización) en **VCOT**   


##  [**Cómo relacionar un pedido a una factura**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#cómo-relacionar-un-pedido-a-una-factura)   

Ingresamos a la aplicación **Pedidos - VPED**.  En esta aplicación se consulta el pedido por cualquier campo que se desee.  Cuando ya se tenga el registro, se va al campo **_Status_**; para poder realizar la factura, se debe liberar la retención del pedido, para esto, se consulta la aplicación **Pedidos retenidos - COPR**, aquí también se puede consultar por cualquiera de los campos.  En esta aplicación se encuentran 6 botones idénticos pero todos tienen una función diferente: el primer botón **_Libera Cartera_**, el segundo **_Devuelve cartera_**, el tercero **_Rechaza cartera_**, el cuarto **_Libera comercial_**, el quinto **_Devuelve comercial_** y el sexto **_Rechaza comercial_**.  Como el pedido en este caso tiene el Status **_Libera comercial_**, se elige este botón, al seleccionar esta opción, desaparece el registro.  

![](vped56.png)  

![](vped57.png)  

![](vped58.png)  

![](vped59.png)  

![](vped60.png)  


Ahora se regresa al pedido en la aplicación **Pedidos - VPED**, se refresca la aplicación y el Status cambia a **_Pendiente por despacho_**, es decir que ya quedó liberado del _Retenido por comercial_, cabe aclarar que esta _Retención_ es parametrizable, en este caso depende totalmente de la empresa y de la parametrización que esta tenga; si la empresa no tiene ningún tipo de _Retención_ parametrizada, se puede omitir este paso.  

![](vped61.png)  


Ahora se procede a crear la factura.  Para esto, se ingresa a la aplicación **Facturas - FFAC** y se adiciona un nuevo registro (+), se diligencia el campo **_Documento_** donde mediante el Zoom se puede elegir la opción **_FC_** de Factura de ventas, **_Ubicación Cero (0)_** y en el **_Concepto_** también se elige la opción **_FC_** Factura Clientes, campo **_Motivo Cero(0)_** y en el campo **_Tercero_** se le elige el mismo tercero con el que se realizó el pedido.  

![](vped62.png)  


En este momento se pasa a relacionar la Factura con el Pedido.  Este proceso es exactamente igual al de Relacionar una Cotización con un Pedido: se diligencia el campo **_Documento1_** (se verifica el documento del pedido en **Pedidos - VPED**, luego, el campo **Ubicación1_** que también se verifica en **Pedidos - VPED_**; diligenciados estos dos campos, se abre el Zoom en el campo **_Número1_** y se selecciona el Pedido realizado.  Diligenciados estos campos, se guarda el registro.  Y finalmente, se procesa la Factura.  En este momento se puede apreciar que el proceso fue satisfactorio.  

![](vped63.png)  


![](vped64.png)  

## [**Pedidos con separada**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#pedidos-con-separada)  

En esta sección, se explica el manejo de la mercancía separada y su efecto en la factura de venta.  Es importante tener en cuenta que este proceso aplica en las empresas que cuentan con varios vendedores, que realizan pedidos de mercancía desde diferentes ubicaciones y necesitan reservar o apartar una determinada cantidad de producto para asegurarse que no vaya a ser apartada o vendida por otro vendedor.  El primer paso es asegurar que la parametrización donde se van a realizar el pedido y la factura se encuentre correcta.  La forma correcta es que en la aplicación **Ubicaciones Organización - BUBI**, el campo _Separada_ debe estar con el _check_ activado.  

![](vped65.png)

Luego, se procede a realizar el pedido.  Se adiciona un nuevo registro (+).  En el campo _Documento_ se escribe **_PD_** de Pedidos; en el campo _Ubicación_, la ubicación definida; en el campo _Concepto_ **_PD_** de Pedidos; en el campo _Cliente_, el número de documento del cliente; se guarda el registro.

![](vped66.png)  

En el detalle, en el zoom del producto, se da click derecho, escogiendo la opción _Ver saldo por Ubicación detallado_  

![](vped30.png)  

Aquí, se toma el producto que se desea. Para la ilustración, hay 119 unidades disponibles del producto escogido, se separan 10 unidades. 

![](vped31.png)  

![](vped32.png)

Se adiciona en el registro. En el detalle queda agregado correctamente.  

![](vped33.png)  

![](vped34.png)

Después se procesa.  

![](vped35.png)  

Posteriormente, se ingresa a la aplicación **Aprobación de Pedidos - VPPR** y con el número del pedido, se hace la aprobación.  Se hace click en el tercer botón: _Aprueba_Pedido_.  

![](vped68.png)  

Ahora se ingresa a la aplicación **Facturas - FFAC** para crear la factura.  En el campo _Documento_, **_FC_** de Factura de venta, en el campo _Ubicación_, la misma ubicación; en el campo _Concepto_, **_FC_**; en el campo _Tercero_, el mismo cliente del pedido.  En la parte inferior, se procede a relacionar el Documento. En el campo _Documento1_, **_PD_**, en el campo _Ubicación1_, la misma ubicación; en el campo _Número1_, el número del pedido.  Se llena también el campo _Condición de pago_ y se guarda el registro.  El sistema hereda en el detalle, la misma información del pedido. Se revisa la respectiva parametrización en las pestañas _Detalle_ y _Pago_ y se procesa la factura.  

![](vped69.png) 

![](vped70.png) 

Se puede confirmar que luego de procesado el pedido, se había actualizado el campo _Separada_ en el detalle a Diez (10).  Se actualiza el mismo documento y ahora el campo se actualiza a la cantidad Cero (0), debido a que la cantidad ya no está separada sino facturada.  

![](vped71.png)  

![](vped72.png)  


## [**Monto mínimo en un pedido**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#monto-mínimo-en-un-pedido)

Proceso correcto, se debe tener la siguiente parametrización:  
Desde la opción **BCON** (conceptos) se debe buscar o agregar el concepto del pedido, para este caso utilizaremos el CA (Catalogo).  
Importante, en el  **BCON** se debe tener parametrizado en el campo: **Clase** como **Monto Mínimo**  

![](bcon1.png)  

* Parametrización del tercero del pedido:  
En el **BTER** se busca en el Tab de Seguridad sobre el campo Nivel de Autorizacion que para este caso es el numero cero (0).  

![](bter1.png)  

* Rangos o montos.  
En el **BRAN** se busca por el documento, Concepto y el campo alcance según el nivel de autorización y según el campo mínimo se valida si el total del pedido es mayor al valor del campo mínimo para procesar correctamente.  

![](bran1.png)  

* Según la parametrización realizada solo se puede procesar el pedido **VPED**,
 Si el monto supero los 200.000, caso contrario el sistema devuelve un mensaje de control, indicando los valores del documento y el rango parametrizado en **BRAN** (Rango)   
 
 ![](bran2.png)  
 
 ![](vped35_01.png)  

**De esta forma se controla para: "no recibir pedidos con rangos inferiores a (xxx.00) monto o rango".**


## [**Actualizar Datos de Cliente**](http://docs.oasiscom.com/Operacion/scm/ventas/vpedido/vped#actualizar-datos-de-cliente)

En la opción **WVAR** se debe crear la variable ***VPEDVALClient***, si el valor del campo Formula es **1** se activará la alerta de actualizar datos del cliente al momento de crear registros nuevos dentro de la opción **VPED**.
 ![](vped15.png)  

Se ingresa a la opción **VPED** y se procede a realizar la creación de un nuevo registro allí podemos observar que se muestra una alerta de notificación informativa al usuario indicando que debe actualizar los datos del cliente.
 ![](vped16.png)  