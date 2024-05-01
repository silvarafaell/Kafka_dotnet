### Curso Apache Kafka + .Net Core - Udemy 

- Apanhe Kafka grava as mensagens em disco, em arquivo binários, forma assincrona.

## Principais Caracteristicas
- Platadorma de steaming de dados distribuida e de codigo aberto
- Projetada para lidar com grandes volumes de dados em tempo real
- Atua coo um sistema de mensageria altamente escalável e durável
- Arquitetura distribuida permite facil escalabidade horizontal
- Amplamente utilizado em casos de uso como o processamento de eventos em tempo real, integração de sistemas e análise de dados em tempo real.

## Arquitetura do Kafka
- Zookeeper
- Produtores
- Kafka cluster
- Consumidores
- Grupo de consumidores

## Broker 
- Servidores que armazenam e gerenciam as partições dos tópicos no kafka
- Constituem o cluster Kafka e são responsaveis por receber, armazenar e replicar os dados
- Escabilidade horizontal e Replicação de dados

## Topico
- Canais de comunicação categorizados para dados no kafka
- Produtores enviam mensagens para topicos, consumidas por consumidores e Tópicos podem ter multiplas partições para distribuição e paralelismo. 
- Tópicos é divididos em partições
  
## Produtor
- Responsavel por enviar dados para o kafka
- Envia mensagens para o topicos kafka de forma assincrona ou síncrona
- Anteriormente não era possivel fazer ordenação

## Consumidor
- Aplicativos ou sistemas que recebem e processam os dados do kafka
- Os consumidores se inscrevem nos topicos para receber mensagens e processá-las conforme necessário e Podem ser implementados em diferentes linguagens e poddem ser configurados para consumir mensagens de forma síncrona ou assíncrona.
- Flexibilidade na configuração do comportamento de consumo, como controle de offset e commits automáticos e capacidade de dimensionamento para lidar com grandes volumes de mensagens
- avisa o kafka que leu a mensagem

## Grupo de consumidores
- Conjuntos de consumidores que compartilham a carga de processamento dos dados no kafka
- Os consumidores são organizados em grupos para consumir dados de tópicos especificos e cada mensagem é processada por apenas um consumidor dentro do grupo, garantindo a distribuição equitativa da carga
- Ideal para lidar com volumes significativos de mensagens

## Zookeeper
- Ferramenta de coordenação distribuida amplamente utilizada em sistemas distribuidos
- Coordenação de Broker
- Registro de metadados
- Detecção de Falhas
- Coordenação de consumidores
- Sincronização de configuração

## Abrindo cmd no direitorio do arquivo docker compose 
   - docker-compose up -d (executa os containers)

## Kafdrop
- depois executa o docker-compose, pode abrir o kafdrop http://localhost:9007/

  
