---
title:
- Padrão de Projeto: Chain of Responsability
author:
- Alexandre Fabian
theme:
- Copenhagen
fontsize:
- 12pt
---

# Padrão:

\Huge Chain of Responsability\par

# Chain of Responsability

\Large É um padrão de projeto comportamental\par

# Características

1. \Large  Permite que se passe requisições por uma corrente de processamento. \par
   

2. \Large O Padrão é composto de um objeto de cliente e um grupo de handlers.  \par

# ...  
3. \Large Evita o acoplamento do remetente ao receptor, ao dar a mais de um objeto a oportunidade de tratar a solução (GAMMA et al., 2000) \par


# Handlers

- \Large Cada Handler trata (ou não) a requisição.\par
  
- \Large Decide se passa para o próximo ou quebra a corrente.\par

# ...

- \Large Reduz a complexidade do problema. \par
  
- \Large Deixa os objetos mais simples. \par

# Quando Aplicar

- \large Quando mais de um objeto precisa processar uma requisição; \par
  
- \large os handlers precisam de uma ordem especifica para serem executados; \par
  
- \large os handlers utilizados e sua ordem podem ser mudados dinamicamente. \par


# Vantagens

- \Large É possivel controlar a ordem que a requisição irá passar pelos handlers. \par
  
- \Large Princípio de Responsabilidade Única. \par
  
- \Large Princípio do Aberto/Fechado. \par

# Desvantagens

- \Large Algumas requisições podem ficar sem tratamento. \par

# Como aplicar

- \large Declarar uma **interface** para o Handler; \par
- \large um Handler **base** com código comum aos demais; \par
- \large os Handlers **concretos**; \par
- \large e o **Cliente** que irá compor a corrente. \par

# Exemplo

\Large Sobre o exemplo:  \par
- \large Revision Web Service: Serviço para revisão de exercício de
programação realizado no Github e registro de nota no Moodle. \par

# Exemplo
![Chain do Projeto Revision](chain.png)

# Exemplo
![Lista de Checkers](listaCheckers.png)

# Exemplo
![Exemplo de Checker Concreto](checkerConcreto.png)

# Referências

- https://github.com/orion-services/revision

- SHVETS, Alexander. Dive Into Design Patterns. Kamianets-Podilskyi, Ucrânia. Refactoring.Guru, 2019. 409 p.

- GAMMA, Erich; JOHNSON, Ralph; HELM, Richard; VLISSIDES, John. Padrões de Projetos: oluções reutilizáveis de software orientados a objetos. São Paulo: Bookman, 2000. 360 p. Tradução Luiz A. Meirelles Salgado.