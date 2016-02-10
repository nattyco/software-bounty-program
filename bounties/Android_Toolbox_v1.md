![alt text](https://github.com/bitDubai/media-kit/blob/master/MediaKit/Fermat%20Branding/Fermat%20Logotype/Fermat_Logo_3D.png "Fermat Logo")

# Android toolbox  V1 (The first bounty for DEVELOPERS AND GRAPHIC DESIGNERS!!!!)

## Introduction

Fermat es una aplicación compleja que corre sobre nuestro propio framework de desarrollo, nos encontramos en una capa sobre el sistema operativo, en este primer momento estamos desarrollando sobre android, por lo cual, se deben crear las bases para poder facilitar y agilizar la creación de aplicaciónes en nuestra plataforma.

Se deben desarrollae las bases, componentes,vistas,utilidades y optimizadores para poder llegar a un nivel de abstracción superior, dejando de pensar en lenguajes de programación y comenzando a pensar en componentes, comenzando por el más bajo nivel del framework y subiendo hasta componentes ya contruidos y preparados para su uso.

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
|notificationes	| template de notificaciones |	furszy |	view |
|BitcoinPicker |	selector de los diferentes montos de bitcoin (mili,micro,satoshis,etc) |	furszy |	dialog,popup,fragmento |
|MoneySelectorDialog |	selector de monedas de los diferentes países |	Luis |	dialog,popup,fragmento |
|SettingsView |	diseño de vista para el settings de cualquier aplicacion fermat |	furszy	| Componente |
|IdentitySelector|	Un view para seleccionar identidades (en las communities/wallets por ejemplo). Que se pueda trigger desde por ejemplo el header del navigationDrawer |	abicelis |	view?|
|FermatAdapter 2.0 |	Mejorar el fermat adapter para que sea mas sencillo agregar cosas como footers y headers, terminar de implementar la capacidad de usar tipos |	nelsonalfo |	Adapter|
|fermatViewHolder 2.0 |	Mejorar el view holder con lo nuevo del adapter|	furszy|	ViewHolder|
|SendForm |	desarrollar una vista envió de dinero|	furszy|	view|
|FermatLoadingView |	una view de loading con estilo de fermat |	furszy|	view|
|FermatSearchView |	SearchView en el toolbar con collapse y expand	|furszy/no se quien la pidió |	view |
|ImageSlider |	un slider con imágenes optimizado para android |	furszy |	
|cuadro de dialogo |	cuadro de dialogo que permita pasarle un objeto y este lo implemente dentro de el, ejemplo si le lapso una lista que es cargue un combox, asi el usuario escoge una opcion y devuelve lo que eate escogio, la idea es que se le pase el titulo, el objeto y que el componente haga el resto. |	miguel payarez |	dialog, popup|
|Simplificación del NavigationStructureFactory |	Desarrollar una alternartiva a la implementación actual que obligue a "setear" todos los elementos obligatorios, así evitaríamos que nos olvidemos setear valores importantes. |	Furszy: (Esto va a ser por defecto con los valores basicos) |	improve|
|basic menu in drawer with header picture V2 |	el navigation view, todo estandarizado |	furszy |	improve|
|top toolbar expandible menu |	hacer el menú que se expanda del icono de la derecha a nivel de más arriba |	furszy |	view |
|animación entre pantallas |	La posibilidad de agregar un efecto al pasar de pantalla en pantalla en una FermatApp |	nelson |	animation|
|QR scanner for everybody V2 |	El scanner de qr hacerlo más simple para su uso en cualquier aplicación | 	furszy |	new functionality |
|Grafico de barras para el header (como el de CBP) |	Hacer el gráfico de barras de cbp para todo fermat |	nelson |	Componente|
|Grafico lineal para el header (como el de CBP) |	Hacer el gráfico lineal de cbp para todo fermat |	nelson |	Componente|
|SimpleSpinnerView with material design |	Un spinner para crear facilmente con material design	| furszy |	Componente|
|FermatFlipAnimation |	Animación especifica para rotar una tarjeta para cualquier container |	furszy |	Animation|
|FermatFlipCard |	Un container el cual pueda rotarse y tenga de ambos lados información diferente para el usuario |	furszy |	Componente |
|ImageCompressor |	Compresor de imágenes al nivel de que no se pixelen y se puedan transferir de una forma más sencilla |	furszy |	Utilidad|
|fermatCryptoCurrencieExchange widget |	un widget para el inicio de android con el valor del bitcoin de fermat |	furszy	| widget |
|TransactionsFragment |	ventana de transacciones con valores básicos como lo son: el sender, destination, amount, date, description	| furszy |	 componente|
|contactsFragment |	ventana de contactos con valores básicos como lo son: el nombre, la imagen.	|furszy | componente|
|FermatProgressBar |	una barra de progreso que se pueda actualizar facilmente desde las notificaciones |	acostarodrigo | view |
|WalletSelectorDialog |	un selector de wallets dentro de fermat, con el cual se va a poder realizar alguna acción al clickearla |	furszy | view|


 *Luis, de todos estos componentes tengo una lista a parte con estado de los mismo, quien los está armando y quien tiene prioridad (la prioridad la pongo yo si se tardan los que dieron la idea).
---


***Once approved, each element will have a better description in the documentation***
     

## Timeline

Based on current workload and resouces available, the delivery date of this bounty will be **March 15th**.

## Evaluation

To be considered success this bounty must pass the following tests:

* All of the components have to been created and finished.

* La evaluación que se realizará será en base a lo aportado, sean diseñadores gráficos o desarrolladores. Se realizará un calculo matematico para determinar cuanto a sido el aporte de la persona para completar el bounty en base a la cantidad de componentes realizados con exito.
* El dueño de la idea , como ya lo fuí explicando a cada uno que quiso aportar, tendrá la prioridad del desarrollo del componente ante el responsable de llevar a cabo este bounty , si el dueño de la idea se encuentra ocupado a la hora de su creación y hay otra persona libre, el organizador del bounty puede determinar la importancia del componente y si es necesario, entregarselo a la otra persona para su desarrollo, ganando así los tokens del mismo.

*[Evaluation results to be completed after evaluation]*

## Distribution

*[Distribution to be completed after evaluation]*
