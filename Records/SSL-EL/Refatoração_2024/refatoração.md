# Refatoração do sistema 2024

Com a competição de 2023 a equipe percebeu que não consegue trabalhar eficientemente com o código atual. A partir disso foi decidido fazer uma refatoração do código visando as seguintes melhorias:
- Garantir que código funcione
- Melhorar a legibilidade do código
- Criar documentação
- Modularizar o sistema
- Implementar boas práticas de desenvolvimento

# Modularização do sistema

Buscando diminuir a complexidade do sistema, tornar mais fácil fazer mudanças no futuro e tornar o sistema mais fácil de se entender foi decidido criar módulos que sejam o mais independete possível um dos outros.

Os módulos decididos foram:
- Visão
- Estratégia
- Movimentação
- Controle
- Comunicação
- Interface
- Juiz
- Intermediador

Para que fosse possível realmente isolar cada um dos módulos teremos que ter uma nova entidade que faz a comunicação entre eles, o itermediador

A ideia é fazer com que todos os possíveis nós de cada módulo estejam dentro de um pacote com esse nome, assim centralizando partes similares e melhorando a organização do código.

# Test Driven Development

Para garantir que o código funcionará independente das mudanças que fizermos agora e no futuro adotamos o TDD como técnica de desenvolvimento.

Outro grande benefício de usar TDD e testes unitários é que eles funcionam como uma documentação que é atualizada quase que naturalmente, não precisando criar outro hábito de atualizar a docuemntação sempre que fizermos uma mudança no código.