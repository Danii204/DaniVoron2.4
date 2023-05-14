# DaniVoron 2.4
Este es el repositorio oficial que recopila toda la información sobre la construcción de una impresora 3D por Daniel Acevedo Facal, como proyecto opcional de la asignatura de Proyectos Integrados 1 de la carrera de Robótica en la USC.

## Introducción
Este proyecto se inició con la intención de diseñar una impresora 3D propia. Después de una gran búsqueda de información, llegué a la conclusión de que lo más inteligente era construir un proyecto de código abierto. Estos proyectos Open Source tienen una gran comunidad que puede ayudarte en caso de que tengas algún problema. Además, existen muchas modificaciones disponibles para mejorar la calidad y velocidad de la máquina.

## Elección de la impresora
Como se mencionó anteriormente, se decidió construir una impresora 3D de código abierto. Después de realizar una exhaustiva búsqueda de información, se optó por construir una impresora 3D del tipo CoreXY debido a su gran velocidad y precisión, así como a su diseño compacto. Tras evaluar diferentes opciones de impresoras de este tipo, se decidió construir una Voron 2.4, ya que cuenta con un diseño compacto y una gran comunidad detrás. Además, existen una gran cantidad de modificaciones disponibles para mejorar la calidad y velocidad de la máquina.

## Elección de los componentes
Para la elección de los componentes se tomaron en cuenta las recomendaciones de la comunidad de Voron. Se optó por utilizar una placa Octopus v1.1 con drivers TMC2209, los cuales son muy silenciosos y tienen una gran calidad. Además, la placa cuenta con una gran cantidad de pines disponibles para conectar diferentes componentes. Para la fuente de alimentación, se eligió una fuente de 24V y 350W, que es más que suficiente para alimentar la impresora. Para el extrusor, se decidió utilizar un extrusor BMG y para el hotend, se eligió un hotend V6. Cabe destacar que no se compró el hotend original, lo que generó problemas con los tamaños, la calidad y el flujo de la impresora. Para los motores, se optó por utilizar motores Nema 17 de 0.9º, los cuales cuentan con una gran cantidad de par. En cuanto a los sensores, se decidió utilizar un sensor inductivo de la marca Omron para la nivelación, ya que es muy preciso y de gran calidad. Para la cama, se decidió utilizar una cama de 300x300mm. Para la electrónica, se eligió una Raspberry Pi 3b, que permitió instalar Mainsail OS (un sistema operativo específico para impresión 3D), así como usar el firmware Klipper. El marco de la impresora está construido con perfiles de aluminio tipo B de 20x20mm, los cuales permiten acoplar las partes de la impresora con facilidad con Tnuts. Las piezas de impresión 3D están impresas en PLA, aunque se reemplazarán en el futuro por piezas impresas en ABS para una mayor resistencia a la temperatura, así como para proporcionar un poco de flexibilidad a la estructura.

## Elección del firmware
Inicialmente, se pretendía utilizar un arduino MEGA con una Ramps 1.4, lo que obligaba a usar Marlin como firmware. Sin embargo, durante el proceso de construcción se descubrió que el uso del arduino Mega + Ramps 1.4 era una mala decisión, por lo que se compró la placa base Octopus v1.1 y la Raspberry 3B, lo que permitió usar Klipper como firmware. Klipper es un firmware que se ejecuta en la Raspberry y se comunica con la placa base. Este firmware es muy potente y permite una gran cantidad de configuraciones. Además, permite una gran cantidad de modificaciones para mejorar la calidad y velocidad de la impresora.

## Elección del software de impresión
Para el software de impresión, se decidió utilizar MainsailOS, el cual es un software específico para impresión 3D. Este software se ejecuta en la Raspberry y permite controlar la impresora desde un navegador web. Además, permite el uso de Klipper.

## Retos durante la construcción
Durante la construcción de la impresora, se encontraron varios problemas. El primero de ellos fue la elección del hotend. Se compró un hotend V6, pero no era el original, por lo que no se ajustaba a las piezas de la impresora. Esto generó problemas con los tamaños, la calidad y el flujo de la impresora. Además, se tuvo que modificar el diseño de la impresora para poder utilizar el hotend.

Aunque el mayor reto fue el tiempo, el cual me presionó fuertemente ya que la mayoría de las piezas proceden de China y los envíos son de al menos 15 días.

## Bibliografía
- [Voron Design](https://vorondesign.com/voron2.4)
- [Voron Documentation](https://docs.vorondesign.com/)
- [Voron Github](https://github.com/VoronDesign)
- [Elli's Print Tuning Guide](https://ellis3dp.com/Print-Tuning-Guide/)