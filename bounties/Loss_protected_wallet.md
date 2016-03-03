![alt text](https://github.com/bitDubai/media-kit/blob/master/MediaKit/Fermat%20Branding/Fermat%20Logotype/Fermat_Logo_3D.png "Fermat Logo")

# Loss Protected Wallet

## Introducción

Its main goal is to protect the user from losing money when attempting to spend Bitcoins at a price lower than the price when that Bitcoin amount was first purchased (or entered the wallet).
The new functionalities include:
* Storing the exchange rate when a BTC amount is received in the wallet
* Checking the exchange rate when the user attempts to spend an amount of BTC and freeze the funds if they are below the purchased price

The Fermat book chapter related to this bounty can be found here: https://github.com/Fermat-ORG/fermat-book/blob/master/book-chapter-12.asciidoc

## Scope

## General Purpose

Desarrollar la app Loss Protected Wallet que sera parte de la capa CCP y reutilizara componentes ya realizados como Network Services, modulos transaccionales y modulos de contactos.
Tendra como funciones basicas:

  * Hacer un pago en BTC (enviar bitcoin a un contacto)

  * Recibir pagos en BTC

  * Mostrar transacciones

  * Mostrar el balance de la  billetera
  
  * Mostrar la cotizacíon actual en dolares del bitcoin.
  
  * Impedir que el usuario envie btc si la cotización actual es menor a la cotizacion del ultimo ingreso de btc a la billetera.

  * Mostrar una lista básica contactos (de nombre de usuario y la dirección de su bitcoin wallet)
  
  * Poder hacer una transferencia de la Reference Wallet a esta wallet y viceversa, a traves de un nuevo modulo transaccional de intercambio de btc intra device.
  
  * Mostrar en una pantalla la informacion estadistica de los ingresos en btc, cada uno tomado como una unidad que se irá dividiendo si es necesario para ir consumiendo la totalidad de los inputs de la transacción original.

 
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



### Bounty scope

#### Objetivos a cumplir
Se desarrollarán los siguientes componentes:
 * App Loss Protected Wallet: aplicacion de android que permitira al usuario hacer uso de las funciones de esta wallet.
 * Module Loss Protected Wallet: que conectara la app de Android con el resto de los plugins.
 * Basic Loss Protected Wallet: plugin que guardara la informacion de las transacciones de la wallet, balance y cotizaciones.
 * Desarrollar un modulo transaccional de intercambio de btc intra device.
 * Desarrollar la funcionalidad para poder tomar cada btc de la wallet como una unidad que se ira dividiendo si es necesario para ir consumiendolos en base a la evaluación de la cotización original con la que ingresaron los fondos y la cotización al momento de consumirlos.



## Timeline

Sobre la base de la carga de trabajo y los recursos actuales disponibles, la fecha de entrega de esta recompensa (bounty) será **31 de Marzo**.

## Evaluation

Para ser considerado éxitoso esta recompensa (bounty) debe superar lo siguiente:

* Todos los elementos anteriormente expuesto deben ser realizados.

* La evaluación que se realizará será en base a lo aportado, por cada uno de los desarrolladores. Se realizará un calculo matemático para determinar cuanto ha sido el aporte de la persona para completar el bounty en base a la cantidad de elementos realizados con éxito.

*[Evaluation results to be completed after evaluation]*

## Distribution

*[Distribution to be completed after evaluation]*


