
###API Gateway URL

https://localhost:8765/{application name}/{uri}

http://localhost:8765/currency-exchange-service/currency-exchange/from/USD/to/INR
http://localhost:8765/currency-exchange-service/currency-exchange-feign/from/USD/to/INR

http://localhost:8765/curreny-conversion-service/currency-converter-feign/from/EUR/to/INR/quantity/10

RABBIT_URI=amqp://localhost java -jar zipkin-server-2.21.0-exec.jar