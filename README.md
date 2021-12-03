# LHCb-GAN
Fast simulations for the LHCb calorimeter (July 2021)


A lo largo del periodo [Marzo-Julio+] realicé contribuciones para el equipo de altas energías de la UB en colaboración con el grupo CERN y el grupo de apoyo al CERN de la Universidad de Cincinnati.

## CONTEXTO A LA FÍSICA DE PARTÍCULAS

Un papel importante para entender las colisiones que se generar en los aceleradores de partículas como el LHC es la producción de simulaciones. Gracias a las simulaciones los físicos somos capaces de reproducir las colisiones entre protones y otras partículas subatómicas y entender la estructura fundamental de la materia así como dar respuesta a preguntas fundamentales de la física hoy sin responder, como lo pueden ser la explicación de la asimetría materia/antimateria o la violación CP de la conjugación y paridad de carga.

Para hacernos una idea, el 80% de los recursos globales computacionales del CERN son destinados a la realización de simulaciones. Existen avanzadas técnicas de optimización de simulaciones para dismunir los costes computaciones (como las técnicas basadas en los niveles Trigger), sin embargo, el volumen de datos generado sigue siendo del orden de los 40GB/s, lo cual produce una ingente cantidad de datos muy difíciles de manejar, gestionar, y estudiar.

Para el año 2022 el LHC recibirá actualizaciones, entramos en la fase 'High Lumi' que estima se triplicarán la cantidad de datos recogidos de las simulaciones, esto va a suponer unos retos computacionales a día de hoy sin precedentes, los mayores volúmenes de datos recogidos del mundo.

Ante este panorama actual y por venir, los actuales métodos de simulación (basados en Montecarlo) son insuficientes y extremadamente costosos, ya no solo en uso de GPU's, sino en los tiempos necesarios para ejecutar una única simulación.

Nace la necesidad de explorar nuevas técnicas que permitan acelerar los tiempos de simulación y minimizar los costes de computación.

Así pues, a lo largo de este periodo de trabajo se emplearon las GAN (Generative Adversarial Networks). Las GAN son redes neuronales artificiales que son capaces de generar imágenes realistas y teóricamente pueden suponer unos costes de simulación 5 órdenes de magnitud menores que los costes de las simulaciones actuales (Montecarlo).

La primera prueba constatada de la efectividad y el enorme interés y potencial de esos modelos generativos basados en redes neuronales profundas (perceptrón multicapa) es la que se aporta en el presente trabajo.

Para un conocimiento más profundo y formal sobre el sustento teórico de las GAN (o variantes como las cGAN, WGAN,etc) se adjunta el artículo oficial donde se detalla el funcionamiento de estas redes neuronales así como el contexto teórico de su funcionamiento. El artículo oficial se puede encontrar de manera gratuita en: https://arxiv.org/abs/1406.2661
