# Curso de Docker

# Domain Driver Design (DDD)

#### O que é DDD ?

- É uma forma de desenvolver com o foco no coração da aplicação , o que chamamos de domínio
  tendo o objetivo de enteder suas regras,processos e complexidades, sepadando-as assim de outros pontos
  complexos que normalmente são adicionados durante o processo de desenvolvimento.

#### Onde veio o DDD?

- Ele veio através do Eric Evans em 2003

#### Softwares complexos

- DDD é / deve ser aplicado para casos de projetos de softwares complexos
- Grandes projetos possuem muitas areas, muitas regras de negócio, muitas pessoas com diferentes visões em diferentes contextos.

#### Como o DDD pode ajudar?

- Entender com profundidade o domínio e o subdomínio da aplicação
- Clareza do que é complexidade de negócio e complexidade técnica

#### Entities

- "Uma entidade é algo unico que é capaz ser alterado de forma continua durante um longo período de tempo." by: Vernon
- Sempre auto validar

#### Value Objects

- "Quando você se preocupa apenas com os atributos de uma elemento de um model, classifique isso como um Value Object"

- "Trate o value object como imutavel"

#### Agregado

- "Um agregadpo é um conjunto de objetos associados que tratamos como um unidade para propósito de mudança de dados"

#### Domain Services

- "Um serviço de domínio é uma operação sem estado, que cumpre uma tarefa específica do domínio.Muitas vezes,a melhor indicação de que você deve criar um Serviço no modelo de domínio équando a operação que você precisa executar parece não se encaixar com um método em um Agregado (10) ou um Obejtco valor(6)


### Comandos

Iniciar o node

- npm init

Compilar na pasta /dist

- npx tsc

Install typescript

- npm i -D typescript
- npx tsc --init

Install Lint

- npm i -D tslint
- npx tslint --init
