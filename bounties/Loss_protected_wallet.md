![alt text](https://github.com/bitDubai/media-kit/blob/master/MediaKit/Fermat%20Branding/Fermat%20Logotype/Fermat_Logo_3D.png "Fermat Logo")

# Loss Protected Wallet

## Introducción

Its main goal is to protect the user from losing money when attempting to spend Bitcoins at a price lower than the price when that Bitcoin amount was first purchased (or entered the wallet).
The new functionalities include:
* Storing the exchange rate when a BTC amount is received in the wallet
* Checking the exchange rate when the user attempts to spend an amount of BTC and freeze the funds if they are below the purchased price

Al momento de gastar los btc la app evaluara si la cotización actual es mayor a la cotización guardada para el ultimo ingreso de btc a la wallet, y permitira ir gastando los bloques de valor empezando por el que tenga la cotización más alta primero para continuar consumiendo los siguientes bloques de valor de menor cotización.

The Fermat book chapter related to this bounty can be found here: https://github.com/Fermat-ORG/fermat-book/blob/master/book-chapter-12.asciidoc

## Scope

## General Purpose

Desarrollar la app Loss Protected Wallet que sera parte de la capa CCP y reutilizara componentes ya realizados como Network Services, modulos transaccionales y modulos de contactos.
Tendra como funciones basicas:

  * Hacer un pago en BTC (enviar bitcoin a un contacto)

  * Recibir pagos en BTC

  * Mostrar transacciones

  * Mostrar el balance de la  billetera tanto available como book. El balance available sera calculado en base a los bloques de valor que puede consumir en ese momento teniendo en cuenta la cotización en dolares de los btc.
  
  * Mostrar la cotizacíón actual en dolares del bitcoin.
  
  * Impedir que el usuario envie btc si la cotización actual es menor a la cotizacion del ultimo ingreso de btc a la billetera.

  * Mostrar una lista básica contactos (de nombre de usuario y la dirección de su bitcoin wallet)
  
  * Poder hacer una transferencia de la Reference Wallet a esta wallet y viceversa, a traves de un nuevo modulo transaccional de intercambio de btc intra wallets.
  
  * Mostrar en una pantalla la informacion estadistica de los ingresos en btc, cada uno tomado como una unidad que se irá dividiendo si es necesario para ir consumiendo la totalidad de los inputs de la transacción original.
  
  * Permitir evitar la restricción de proteccion de perdida de btc mediante la selección de un seteo en la configuración de la wallet. Que si esta en true no dejara gastar los btc y si esta en false podra gastarlos.
  


 
 Para esta nueva wallet se necesitaran desarrollar las siguientes componentes:
 
 - Loss Protected Wallet App
 - Loss Protected Wallet Module
 - Basic Loss Protecte Wallet
 - Modulo Transaccional de intercambio de btc intra device

### Current developments in progress

Esta wallet reutilizara las componentes de CCP ya desarrolladas
- Modulos Transaccionales de Incomming y Outgoing
- Plugin de Contactos
- Network Services de envio de metadata.
- Network Services de conexiones entre Fermat Intra Actors
- Network Services de obtención de address de Intra Actors
- Network Services de envio y recepción de Payment Request.
- Modulo de crypto address.
- Modulo de payment request.

Se utilizara la subapp Community para establecer relaciones entre Fermat Users, que despues podran ser agregados como contactos, y la subapp Identity para crear la identidad asociada a la wallet. 

La cotización actual en dolares se obtendra de la componente CBP Crypto World Fiat Index


### Bounty scope

#### Objetivos a cumplir
Se desarrollarán los siguientes componentes:
 * App Loss Protected Wallet: aplicacion de android que permitira al usuario hacer uso de las funciones de esta wallet.
 * Module Loss Protected Wallet: que conectara la app de Android con el resto de los plugins.
 * Basic Loss Protected Wallet: plugin que guardara la informacion de las transacciones de la wallet, balance y cotizaciones.
 * Desarrollar un modulo transaccional de intercambio de btc intra wallets.
 * Desarrollar la funcionalidad para poder tomar cada btc de la wallet como una unidad que se ira dividiendo, si es necesario, para ir consumiendolos en base a la evaluación de la cotización original con la que ingresaron los fondos y la cotización al momento de consumirlos.

#### Workflows

**Envío de Btc**: El usuario de la wallet selecciona la opcion de Send, especifica el contacto al cual hacer el envio y la cantidad de btc, presiona Send. Se verifica el balance disponible para gastar en base a la cotización actual del dolar contra la cotización original de los distintos ingresos de btc.
Si la cotizacion actual es menor se le informara al usuario que no puede hacer el envio ya que perdera dinero, si el seteo de bypass de esta restringcion esta activado se podra hacer el envio de todos modos a pesar de la advertencia. De lo contrario el envio no se realiza.

  Si la cotización es mayor la trasaccion es enviada a traves del modulo transaccional CCP Outgoing Intra Actor Transacction, o   del CCP Outgoing Extra Actor Transacction para contactos externos, al modulo Crypto Vault y se transmite los btc por el        modulo Crypto Bitcoin Network. 

  Se descuenta el monto enviado del balance del la wallet a traves el modulo Loss Protected Basic Wallet quien registra la     transacción. Y se realiza el calculo de cuantos bloques de valor se consumieron en esta transaccion y actualiza el balance  disponible.

  Se envia a traves del NetWork Services Crytpo Transmission la metadata con la información de la transacción a traves del     servidor P2P de Fermat.

**Recepción de Btc**: El modulo Crypto Bitcoin Network informa al modulo Incoming Intra User Transacction, o al modulo CCP Incoming Extra Actor Transacction para contactos externos, que llega una nueva transacción para esta wallet.
Se espera la llegada de la metadata a traves del NetWork Services Crypto Transmission para aplicar la transaccion a traves del modulo Loss Protected Basic Wallet que registra la transacción y consulta la cotización actual de los btc en dolares, para guardar este dato y actualizar el balance disponible.

**Agregar una conexion con un Itra User como un contacto**: Desde la opcion Contactos de la Wallet se podra agregar un nuevo contacto de tipo Fermat User, al elegir esta opción se vera el listado de conexiónes ya realizadas a traves de la sub app Community, si no se tienen conexiones se podra acceder desde este punto a la sub app Community para realizarlas.
Al elegir uno de estos Fermat User de la lista se creara un nuevo contacto para la wallet a traves del modulo Wallet Contact Middleware y se solcitara la wallet address del contacto a traves del NetWork Services Crypto Address el cual envia una solicitud al otro dispositivo a traves de la red P2P de Fermat para que se le retorne la dirección.

- Enviar o Recibir un Requerimiento de Pago
- Denegar un Requerimiento de Pago
- Aceptar un Requerimiento de Pago
- Hacer una transferencia a otra wallet:


#### Wallet Graphic interface
- Home:
      * Resumen de balance available y book
      * Listado de transacciones enviadas y recibidas
- Navigation Drawer: 
       * Identidad: Permite ir a la subapp Identity y modificar los datos cargados, como User Name y foto.
       * Contactos
          * Listado de Contactos
          * Ver Detalle del Contacto con la opcion de hacer un envio de btc o un requerimiento de pago.
          * Agregar un nuevo contacto externo o un Fermat User.
       * Payment Request
          * Listado de Requerimientos enviados y recibidos
          * Hacer un nuevo requerimiento de pago
       * Estadisticas de consumo de los bloques de Valor
       * Settings
           * Enviar Btc a otra wallet
           * Enabled Send Btc Protected
           * Change Networks
- Wallet Toolbar
       * Help
       * Send Btc a contactos
       
    

## Timeline

Sobre la base de la carga de trabajo y los recursos actuales disponibles, la fecha de entrega de esta recompensa (bounty) será **31 de Marzo**.

## Evaluation

Para ser considerado éxitoso esta recompensa (bounty) debe superar lo siguiente:

* Todos los elementos anteriormente expuesto deben ser realizados.

* La evaluación que se realizará será en base a lo aportado, por cada uno de los desarrolladores. Se realizará un calculo matemático para determinar cuanto ha sido el aporte de la persona para completar el bounty en base a la cantidad de elementos realizados con éxito.

*[Evaluation results to be completed after evaluation]*

## Distribution

*[Distribution to be completed after evaluation]*


