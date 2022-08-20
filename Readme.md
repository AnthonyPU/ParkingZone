# Parking Zone

# Posible solución

## General

Este proyecto tiene como finalidad encontrar estacionamientos disponibles en tiempo real por parte del usuario y generar más flujo de clientes para distintos establecimientos que cuentan con zona de parqueo mediante la aplicación “Parking Zone”. Al saber la cantidad de espacios libres podremos tener la certeza de donde conseguir uno de manera eficiente, ahorrar el consumo del combustible y con ello, el decremento de la emanación de CO en la ciudad.

## Hardware

Esto se hará mediante la implementación de un módulo Sipeed que permite reconocimiento de imágenes a través de una cámara y además está integrado con un ESP32 lo que permite la conexión a la red. El procesamiento de la imagen lo hace en el mismo módulo lo que permite reducir tiempo a comparación de realizar ese mismo proceso en el servidor. También cabe decir que el módulo es low-cost y esto no representaría un costo excesivo ni en hardware ni en servicios en la nube, ya que se haciendo referencia a esta última, se utilizaría un arreglo que indica la posición, estado y usuario; información que es de poca cantidad de bytes.

## Nube

En cuanto al servicio en la nube este contará con una base de datos de los usuarios, zonas de parque, estado de cada estacionamiento individual. Todo esto lo integrará a través de una API que permitirá visualizar estos datos tanto en una página web como en una app.

## App

La app, además de visualizar el estado y ubicación de los estacionamientos, también contará con pasarela de pagos para una mayor comodidad por parte del usuario, además se permitirá la opción en efectivo

[Más de 11 mil millones de soles se pierden a causa del tráfico vehicular en Lima](https://rpp.pe/economia/economia/mas-de-11-millones-de-soles-se-pierde-a-causa-del-trafico-vehicular-en-lima-noticia-1413102)

[Plataforma Nacional de Datos Abiertos](https://www.datosabiertos.gob.pe/dataset/indicadores-mensuales-de-trafico-por-tipo-de-veh%C3%ADculo-ene-2019-mar-2022-organismo-0#%7B%7D)

# Arquitectura de solución