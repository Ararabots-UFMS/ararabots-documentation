# Git Flow - Ararabots

## Table of Contents

- [Introdução](#introdução)
- [Analisar](#analisar)
- [Setar Metas](#setar-metas)
- [Criar safety net](#criar-safety-net)
- [Refatorar passo-a-passo](#refatorar-passo-a-passo)
- [Medição de sucesso](#medição-de-sucesso)
- [Referências](#referencias)

# Introdução
Para que a refatoração seja aplicada de maneira que melhore o código é necessário seguir alguns pontos essenciais:
- Analizar
- Setar metas
- Criar safety net
- Refatorar passo-a-passo
- Medição de sucesso


# Analisar

A análise é a primeira etapa da refatoração, que consiste em identificar potenciais problemas no código, os mais comuns sendo:

- Métodos longos
- Classes longas
- “Primitive Obsession”
- Longas listas de parâmetros
- Data Clumps

# Setar Metas

Todo processo de refatoração de um código é guiado por um objetivo específico: Melhorar o código atual. Essa meta somente é alcançada através da definição de metas secundárias, partindo do princípio de divisão e conquista, assim evoluindo o código antigo.

Metas como legibilidade, otimização ou componentização são excelentes pontos de partida para refatorar um código. Dessa forma, facilitando o processo de encontrar possíveis bugs e dando mais qualidade ao código. Vale ressaltar que tais metas precisam ser debatidas pela equipe, assim definindo quais os principais objetivos da refatoração.

# Criar safety net

Durante o processo de refatoração você estará mudando o código e possivelmente criará novos problemas nesse processo. Para que isso não acabe quebrando o código original é preciso ter maneiras de assegurar que o código continua funcionando com as mudanças.

A melhor maneira de garantia é escrever testes que testam todas as funções do código, assim apontando quando uma para de funcionar.

As técnicas de TDD e red-green-refactor são maneiras já muito estabelecidas de fazer exatamente isso.

# Refatorar passo-a-passo

A refatoração possui inúmeras possíveis maneiras de ser executada dependendo dos objetivos a serem alcançados. 
Podemos utilizar dos exemplos de sites como Refactoring Guru para procurar problemas e suas soluções aplicando em nossos códigos.

No nosso caso (SSL-EL 2024), devemos prestar atenção em:
- Níveis de indentações excessivos
- Sequências de if-else’s grandes
- Números “mágicos”


# Medição de sucesso

Analisar se obteve sucesso, verificando se o objetivo que você estabeleceu para si mesmo foi realmente alcançado.


# Referencias

[Refactoring Guru](refactoring.guru)

[Gilded Rose Kata](https://www.youtube.com/watch?v=Rryo6CoKamE)

