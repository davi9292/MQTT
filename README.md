# Projeto MQTT - Publisher e Subscriber em Python

## Descrição

Este projeto é um exemplo simples de comunicação utilizando o protocolo MQTT em Python.
O programa funciona como **publisher e subscriber ao mesmo tempo**, ou seja, ele envia mensagens para um tópico e também recebe mensagens publicadas nele.

## Tecnologias utilizadas

* Python 3
* Biblioteca paho-mqtt
* Broker público HiveMQ

## Configurações utilizadas

* Broker: broker.hivemq.com
* Porta: 1883
* Tópico: senai/pinto

## Pré-requisitos

Antes de executar o projeto, é necessário ter o Python instalado no computador.

Verifique com:
python --version

## Instalação da biblioteca necessária

Instale a biblioteca MQTT com o comando:

pip install paho-mqtt

ou

python -m pip install paho-mqtt

## Como executar o projeto

1. Abra o terminal na pasta do projeto.
2. Execute o arquivo Python:

python nome_do_arquivo.py

3. O programa irá:

* conectar ao broker MQTT
* se inscrever no tópico configurado
* permitir o envio de mensagens pelo terminal
* exibir mensagens recebidas no mesmo tópico

## Funcionamento

O sistema utiliza um broker MQTT público para intermediar a comunicação.
Sempre que uma mensagem é digitada no terminal, ela é publicada no tópico e imediatamente recebida por todos os clientes inscritos, incluindo o próprio programa.

## Estrutura do código

* Configurações do broker e tópico
* Função callback para receber mensagens
* Conexão do cliente MQTT
* Inscrição no tópico
* Loop contínuo para envio de mensagens

## Resultado esperado

Ao executar o programa, será possível enviar mensagens digitadas no terminal e visualizar as mensagens recebidas em tempo real.

## Autor

Davi de Assis Fabricio
