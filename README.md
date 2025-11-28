# tdc_simulacion_tanque
Repositorio para simulacion de TP de Teoria de Control

## Url con aplicación en linea
[Simulación de llenado de tanque de agua](https://pykongroo.github.io/tdc_simulacion_tanque/)

## Ejemplo de uso

### Parametros:
La simulación requiere el seteo de distintos parametros para su uso, la simulación tendrá por defecto los valores indicados en el documento del TP.

Los parametros a configurar se separan en 3 categorias:
#### Parametros variables:
Son aquellos parametros que uno ajustaria en el ambiente real.
Aplicar cambios en estas variables impactaran en la simulacion en tiempo real sin reiniciar la simulacion.
- Altura deseada: Será el nivel del agua que buscamos mantener, será la altura de la boya reguladora.
- Largo del cable: Será la longitud del cable que conecta la boya reguladora con el flotante.

#### Parametros de perturbacion
Son aquellos que permitiran simular una perturbacion en el sistema.
Aplicar cambios en estas variables impactaran en la simulacion en tiempo real sin reiniciar la simulación.
- Amplitud: Será la amplitud de la perturbación, la misma estará expresada en L/s.
- Duracion: Será la duración en la que la perturbación tendrá efecto en el sistema.

#### Parametros no variables:
Son aquellos definidos por el contexto y no son fijos en el ambiente real.
Al impactar el cambio de estas variables, la simulacion se reiniciará.
- Altura total del tanque: Será el nivel máximo de agua que soporta el tanque.
- Diametro del tanque: El diametro de la base del tanque con forma cilindrica.
- Caudal de bomba: El caudal con el que la bomba extractora llenará el tanque de agua, la misma estará expresada en L/min
- Margen de error angular: Será el rango de error con el que el flotante ergulará la activación de la bomba reguladora.

### Funcion de velocidad de simulación:
El panel de control de la simulación cuenta con la funcionalidad de acelerar la simulacion hasta 100 veces, Esta funcionalidad está disponible en forma de otones indicando la velocidad deseada, los cambios de velocidad son en tiempo real, asi que uno podria por ejemplo acelerar la simulacion mientras el tanque empieza el llenado, y luego ralentizar la simulacion para observar mejor los cambios en algun momento deseado.