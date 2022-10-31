---
author:
- Alexandre de Mesquita Fabian
title:
- Padrões de Projeto
fontsize:
- 12pt
theme:
- Copenhagen
---

# Padrão:

Chain of Responsability é um padrão de projeto comportamental

## Características

- Tem como caracteristica permitir  que se passe requisições por uma corrente de processamento, que podem ser chamados de handlers.
- O Padrão é composto de um objeto de **comando** e um grupo de handlers.  

## Handlers

- Cada handler decide se passa para o próximo ou quebra a
corrente, encerrando o processamento nesse ponto, não deixando que os demais membros da corrente percam tempo.

## ...

- Reduz a complexidade do problema a ser tratado por cada
handler.

## ...

- Deixa os objetos mais simples e fáceis de implementar e
manter.

## Quando Aplicar

- Quando mais de um objeto precisa processar uma requisição
- Quando os handlers precisam de uma ordem especifica para serem executados.
- Quando os handlers utilizados e sua ordem podem ser mudados dinamicamente 

## Vantagens

- É possivel controlar a ordem que a requisição irá passar pelos handlers
- Principio da Responsabilidade Única. 
- Principio do Aberto e Fechado, é possível adicionar novos handlers sem quebrar o código existente.

Reduz a complexidade dos objetos e o acoplamento


## Desvantagens

## Como aplicar
## Exemplo

## Referências

- SHVETS, Alexander. Dive Into Design Patterns. Kamianets-Podilskyi, Ucrânia. Refactoring.Guru, 2019. 409 p.

# Apresentação não é apostila.