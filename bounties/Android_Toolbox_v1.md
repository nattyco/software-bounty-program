![alt text](https://github.com/bitDubai/media-kit/blob/master/MediaKit/Fermat%20Branding/Fermat%20Logotype/Fermat_Logo_3D.png "Fermat Logo")

# Android toolbox  V1 (The first bounty for DEVELOPERS AND GRAPHIC DESIGNERS!!!!)

## Introduction

Fermat es una aplicación compleja que corre sobre su propio framework de desarrollo, se encontra en una capa sobre el sistema operativo, en este primer momento estamos desarrollando sobre android, por lo cual, se deben crear las bases para poder facilitar y agilizar la creación de aplicaciónes en nuestra plataforma.

Se deben desarrollae los componentes,vistas,utilidades y optimizadores para poder llegar a un nivel de abstracción superior, dejando de pensar en vistas como codigo si no como componentes ya pre diseñados, comenzando por el nivel más bajo  del framework y subiendo hasta llegar a componentes ya previamente elaborados para su uso.

## Scope

### Current developments in progress

In the present, the toolbox have the basics things to develop in fermat, we have to expand it more with:

## General Purpose

* TextBox
* EditText
* Button
* CheckButton
* BottomSlider
* NavigationView
* Tabs
* Expandable header

### Lists

* Expandable Lists
* RecyclerView

## Dialogs

* Yes / No
* TutorialDialog
* Dialog Welcome Screen / Help Screen
* FermatDialog (Dialog with the fermat basics for custom develop)

## Adapters
* Recycler adapter
* Expandable adapter

### Graphics

* Dona
* Badge (circle with notification number)
* RoundedView
* Picture in Circle

## Workers
* BitmapWorker
* ExecutorWorker

## Tranformation effect
* CircleTransformation

## Inflater
* ViewInflater V1

### Bounty scope

#### Toolbox version V1

Se desarrollarán los siguientes componentes,views,widget,optimizadores,utilidades y mejoras (hace falta acomodarlos por niveles, lo voy a hacer en mi documento y después lo paso acá):

---
| Artefacto  | Descripción  | Idea  | Tipo de vista  |
|:----:|:----:|:----:|:----:|
|ChatView	| fragmento ya pre-armado con lista de chat, burbujas, adapter, holders.|	Luis |	fragmento |
|notificationes	| template de notificaciones y posibilidad de notificaciones custom a traves de un painter |	furszy |	view |
|CoinUnitsPicker |	selector de las diferentes unidades de una moneda, por ejemplo: bitcoin (mili,micro,satoshis,etc) |	furszy |	dialog,popup,fragmento |
|CurrencySelectorDialog |	selector de monedas fiat/crypto  |	Luis |	dialog,popup,fragmento |
|SettingsView |	diseño de vista para el settings de cualquier aplicacion fermat, se debe crear toda la infraestructura para construir esto de forma escalable y fácil de ampliar con diferentes componentes |	furszy	| Componente |
|IdentitySelector|	Un view para seleccionar identidades (en las communities/wallets por ejemplo). Que se pueda trigger desde por ejemplo el header del navigationDrawer |	abicelis |	view?|
|FermatAdapter 2.0 |	Mejorar el fermat adapter para que sea mas sencillo agregar tipos de row,por ejemplo footers , headers, etc. |	nelsonalfo |	Adapter|
|fermatViewHolder 2.0 |	Mejorar el view holder con lo nuevo del adapter para poder almacenar las vistas armadas|	furszy|	ViewHolder|
|SendForm |	desarrollar un formulario de envió básico para todas las plataformas|	furszy|	view|
|FermatLoadingView |	una view de loading con estilo de fermat |	furszy|	view|
|FermatSearchView |	SearchView en el toolbar con collapse y expand	|furszy/no se quien la pidió |	view |
|ImageSlider |	un slider con imágenes optimizado para android (Esto es por ejemplo se puede usar en un header con noticias o alguna información a presentar) |	furszy |	
|Simplificación del NavigationStructureFactory |	Desarrollar una alternartiva a la implementación actual que obligue a "setear" todos los elementos obligatorios, establecer valores por default para evitar mal uso del mismo. |	Furszy/no tengo anotado quien lo sugirió |	improve|
|basic menu in drawer with header picture V2 |	el navigation view, todo estandarizado |	furszy |	improve|
|top toolbar expandible menu |	menú expanpandible desde el toolbar |	furszy |	view |
|animación entre pantallas |	La posibilidad de agregar un efecto al pasar de pantalla en pantalla en una FermatApp |	nelson |	animation|
|QR scanner V2 |	El scanner de qr hacerlo más simple para su uso en cualquier aplicación | 	furszy |	new functionality |
|Grafico de barras para el header (como el de CBP) |	Hacer el gráfico de barras de cbp para todo fermat |	nelson |	Componente|
|Grafico lineal para el header (como el de CBP) |	Hacer el gráfico lineal de cbp para todo fermat |	nelson |	Componente|
|SimpleSpinnerView with material design |	Un spinner para crear facilmente con material design	| furszy |	Componente|
|FermatFlipAnimation |	Animación especifica para rotar una tarjeta para cualquier container |	furszy |	Animation|
|FermatFlipCard |	Un container el cual pueda rotarse y tenga de ambos lados información diferente para el usuario |	furszy |	Componente |
|fermatCryptoCurrencieExchange widget |	un widget para el inicio de android con el valor del bitcoin proporcionado por plugins de Fermat |	furszy	| widget |
|TransactionsFragment |	ventana de transacciones con valores básicos como lo son: el sender, destination, amount, date, description	| furszy |	 componente|
|contactsFragment |	ventana de contactos con valores básicos como lo son: el nombre, la imagen.	|furszy | componente|
|FermatProgressBar |	una barra de progreso que se pueda actualizar facilmente desde las notificaciones |	acostarodrigo | view |
|WalletSelectorDialog |	un selector de wallets dentro de fermat, con el cual se va a poder realizar alguna acción al clickearla |	furszy | view|

---

***Once approved, each element will have a better description in the documentation***
     

## Timeline

Based on current workload and resouces available, the delivery date of this bounty will be **March 15th**.

## Evaluation

To be considered success this bounty must pass the following tests:

* All of the components have to been created and finished.

* La evaluación que se realizará será en base a lo aportado, sean diseñadores gráficos o desarrolladores. Se realizará un calculo matematico para determinar cuanto a sido el aporte de la persona para completar el bounty en base a la cantidad de componentes realizados con exito.
* El dueño de la idea , como ya lo fuí explicando a cada uno que quiso aportar, tendrá la prioridad del desarrollo del componente ante el responsable de llevar a cabo este bounty , si el dueño de la idea se encuentra ocupado a la hora de su creación y hay otra persona libre, el organizador del bounty puede determinar la importancia del componente y si es necesario, entregarselo a la segunda persona para su desarrollo, ganando así los tokens del mismo.

*[Evaluation results to be completed after evaluation]*

## Distribution

*[Distribution to be completed after evaluation]*
