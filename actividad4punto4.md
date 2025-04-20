**`#include <ArduinoJson.h>`**  
Esta línea incluye la biblioteca ArduinoJson.
ArduinoJson es una librería para trabajar con el formato JSON (JavaScript Object Notation) en placas como Arduino, ESP32, ESP8266, etc. 

**`StaticJsonDocument<128> doc;`**  
Se crea un objeto llamado doc de tipo StaticJsonDocument, el cual reserva 128 bytes de memoria estática para almacenar los datos en formato JSON. 
Este objeto servirá como contenedor para construir y organizar la estructura del mensaje JSON.

**`doc["Temperatura"] = temperatura;`**  
 Asigna un valor a la clave "Temperatura" dentro del objeto JSON doc. Esto significa que se esta agregando un nuevo par clave-valor al documento JSON.

**`String jsonOutput;`**  
**`serializeJson(doc, jsonOutput);`**  
**String jsonOutput;** Crea una variable de tipo String llamada jsonOutput que servirá para guardar el texto del JSON que se va a generar.
**serializeJson(doc, jsonOutput);** Convierte el contenido del objeto doc (que es un JSON en memoria) en una cadena de texto. El resultado de esa conversión se guarda dentro de la variable jsonOutput.






