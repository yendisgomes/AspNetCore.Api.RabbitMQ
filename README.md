# Aspnet Core Web API
# Docker
# RabbitMQ

Linha de comando para executar o RabbitMQ em container Docker
docker run -d --hostname rabbitserver --name rabbitmq-server -p 15672:15672 -p 5672:5672 rabbitmq:3-management

1 - Executar o projeto AspNetCore.Api.RabbitMQ
2 - Visualizar o RabbitMQ (http://localhost:15672/)
3 - Utilizar postman / insomnia para enviar o json: 
{
	"OrderNumber": 1,
	"ItemName": "xpto",
	"Price": 20.00	
}

4 - Executar o console AppOrderWorker para consumir a fila orderQueue do RabbitMQ
