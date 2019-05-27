# Kafka-Tweets
Producción, consumición y análisis de tweets en tiempo real.

En Memoria_kafka.pdf pueden encontrarse algunos datos sobre el funcionamiento e instalación de kafka, así como una breve memoria del trabajo desarrollado.

El trabajo está compuesto por cuatro scripts de Python:

- TweetProducer, que colecta tweets mediante la API de Twitter, y los inserta en un topic de Kafka. Será necesario introducir unas claves de acceso a la API de Twitter.
- ConsumerProducer, que obtiene los datos almacenados en el topic anterior, los procesa y los reinserta en un segundo topic.
- TweetsConsumer (Barplor y TimeSeries), que consumen los datos del topic anterior y representan en tiempo real las menciones que se realizan de cada partido político de dos formas diferentes.

REQUISITOS:
- Instalar Apache Kafka y tener en ejecución una terminal con el servidor Zookeeper y otra con el servidor Kafka.
- Obtener unas claves de acceso a la API de Twitter propias (las claves del equipo se han borrado del código).

