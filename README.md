<div align="center">
  <p>
    <img src="./ImgKoywe.png" width="250" />
  </p>
  <p>
    La forma más fácil de comprar o vender crypto en latinoamérica
  </p>
</div>

# Desafío Koywe 

## Introducción

Este es el desafío para aplicar al cargo "Developer" en Koywe.
Contiene 3 secciones para evaluar principalmente habilidades en JavaScript, React, Node.js y TypeScript.

<p>Frontend, Backend y Cuentanos del Desafío </p>

No hay limitaciones más que las expresadas en este documento para realizar el desafío. Puedes hacer uso de componentes, librerías y dependencias que estimes conveniente.

La tarea debe estar contenida en este proyecto, debes clonarlo y realizar tu desafìo en las carpetas ,backend, frontend y en el documento DESAFIO.md

## Front(Full-stack)

Carpeta `/frontend` hay 4 puntos a evaluar:
Construir una pequeña calculadora.

1. En la sección "API desafío Front" se encuentra el endpoint que debes utilizar.
2. Debe contener una tabla donde se listen todos los coins (nombre, imagen, etc)  y current_price entregados por el endpoint.
1. La tabla debe desaparecer cuando se utilicen en smartphone.
2. Debe filtrar contenido el contenido. Implementa los filtros que estimes relevantes

3. Deberá contener una funcionalidad, separada de la tabla del punto 2, que permita calcular el valor de Y current_price para un valor cualquiera de X coins, que se encuentre en el endpoint dado.

4. Debe ser responsive, se evaluará en smartphones, tablet y computadores. Nos interesa ver una buena distribución del espacio en los distintos dispositivos. Que no se pierda la visualización del punto 3 y que aparezca y desaparezca la tabla del punto 2.


**Coingecko API `GET api/v3/coins/` endpoint:**  https://api.coingecko.com/api/v3/coins/


## Backend
### Construcción de una API de Back-end para Criptomonedas utilizando la API de CoinGecko
Carpeta `/backendCoinGecko`. hay 9 puntos a evaluar:

1.**Entender las especificaciones de la API de Coingecko**: Comprender cómo funciona el endpoint `https://api.coingecko.com/api/v3/coins/` y qué datos devuelve.
2. **Creación de la conexión a la base de datos MongoDB**: Utilizando pymongo u otro ORM, establece una conexión con una base de datos MongoDB.
3. **Desarrollo de una función de recuperación de datos**: Crea una función en Python que se conecte a la API de CoinGecko y recupere los datos sobre las criptomonedas.
4. **Almacenamiento de datos en MongoDB**: Almacena el ID de la criptomoneda, el nombre, la imagen y el precio actual en tu base de datos MongoDB.
5. **Creación de endpoints en la API**:
    - ‘/coins’: que retorne todos los datos de criptodivisas almacenados en la base de datos.
    - ‘/coins/<coin_id>‘: que retorne los datos para una cripto específica basada en su ID.
    - ‘/calculate’: que acepte una criptomoneda y una cantidad y devuelva la conversión de esa cantidad a la criptomoneda dada utilizando el precio actual.
6. **Implementación de un mecanismo de programación** para actualizar los precios de las criptomonedas en tu base de datos cada cierto tiempo (por ejemplo, cada 10 minutos).
7. **Pruebas unitarias**: Desarrolla pruebas unitarias para cada función y endpoint para asegurarte de que están funcionando correctamente.
8. **Pruebas de integración**: Realiza pruebas de integración para verificar que todo el sistema funcione correctamente en conjunto.
9. **Documentación**: Documenta tu API, incluyendo cómo ponerla en marcha, cómo usar cada endpoint y cualquier otra información que creas relevante.


## Backend

Carpeta `/backend`. hay 3 puntos a evaluar:

1. Crea una API (REST o GraphQL) con Node.js
3. Debe retornar el crypto-exchange que entregue la mejor oferta de crypto [ETH, BTC] a USD (o USDT), para un monto dado. Sólo ETH, BTC a USD(USDT) usando los "order books".
2. Deberás comparar los crypto-exchange Binance y Coinbase [order books](https://www.investopedia.com/terms/o/order-book.asp) para completar el punto 2.
Ejemplo Tipo
```
GET: http://localhost:4000/best-exchange-usd?amount=10000&crypto=BTC
```

Ejemplo tipo esperado API:

```
{
  "crypto":"BTC"
  "amount": 100,
  "usdAmount": 43240000,
  "exchange": "coinbase"
}
```

#### API Information & Documentation

- **[Binance Order Book API Endpoint](https://github.com/binance/binance-spot-api-docs/blob/master/rest-api.md#order-book)**
- **[Coinbase Order Book API Endpoint](https://docs.cloud.coinbase.com/exchange/reference/exchangerestapi_getproductbook-1)**
- **[Order books, que son y para que sirven](https://wiki.lemon.me/order-books-que-son-y-para-que-sirven/)**
- **[Crypto Trading 101: How to Read an Exchange Order Book](https://www.coindesk.com/crypto-trading-101-how-to-read-an-exchange-order-book)**

### Notas secciones FrontEnd y BackEnd:

-- Impleméntalo como estimes conveniente. En el archivo `DESAFIO.md` , agrega cualquier supuesto y/o consideraciones que hayas tenido que hacer.

- Se dispone de un archivo docker-compose, debes configurar tus apps para que funcionen con él. Será como revisaremos el desafío.


## Cuéntanos del desafío

- Responde las preguntas hechas en el archivo [DESAFIO.md](./DESAFIO.md), son 7.

## Entrega

La entrega la debes enviar en un archivo .zip al correo </p>
`kenneth@koywe.com`

También puedes escribir en caso de dudas, comentarios, errores, etc. Trataremos de responder lo antes posible, pero no en menos de 24 hrs. Debes considerarlo ;)

¡Agradecemos mucho el tiempo que le dedicas al desafío!

Saludos.
