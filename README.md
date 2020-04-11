# Spring Microservices using Spring Cloud

## Application	Ports Used
| Application                       | Ports           |
| -------------                     | -------------   |
| Limits Service                    | 8080, 8081,...  |
| Spring Cloud Config Server        | 8888            |
| Currency Exchange Service         | 8000, 8001,...  |                       
| Currency Conversion Service       | 8100, 8101,...  |
| Eureka Naming Server              | 8761            |
| Zuul API Gateway Server           | 8765            |
| Zipkin Distributed Tracing Server | 9411            |

## URLs

|     Application       |     URL          |
| ------------- | ------------- |
| Limits Service |👉http://localhost:8080/limits|
|Spring Cloud Config Server| 👉http://localhost:8888/limits-service/default 👉http://localhost:8888/limits-service/dev 👉http://localhost:8888/limits-service/qa|
|  Currency Converter Service - Direct Call| 👉http://localhost:8100/currency-converter/from/USD/to/INR//usr/local/var/log/rabbitmq/rabbit@localhost.log/usr/local/var/log/rabbitmq/rabbit@localhost.logquantity/10|
|  Currency Converter Service - Feign| 👉http://localhost:8100/currency-converter-feign/from/EUR/to/INR/quantity/10000|
| Currency Exchange Service | 👉http://localhost:8000/currency-exchange/from/EUR/to/INR 👉http://localhost:8001/currency-exchange/from/USD/to/INR|
| Eureka | 👉http://localhost:8761/|
| Zuul - Currency Exchange & Exchange Services | 👉http://localhost:8765/currency-exchange-service/currency-exchange/from/EUR/to/INR 👉http://localhost:8765/currency-conversion-service/currency-converter-feign/from/USD/to/INR/quantity/10|
|Fault Tolerance Example|👉http://localhost:8080/fault-tolerance-example|

## Installing Rabbit MQ on MAC
https://www.rabbitmq.com/install-homebrew.html
###### Starting Rabbit MQ Server
/usr/local/Cellar/rabbitmq/3.8.3/sbin/rabbitmq-server
###### Rabbit MQ Dashboard
http://localhost:15672/
