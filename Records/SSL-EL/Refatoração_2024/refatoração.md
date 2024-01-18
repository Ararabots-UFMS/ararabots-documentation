# Refatoração do sistema 2024

Com a competição de 2023 a equipe percebeu que não consegue trabalhar eficientemente com o código atual. A partir disso foi decidido fazer uma refatoração do código visando as seguintes melhorias:
- Garantir que código funcione
- Melhorar a legibilidade do código
- Entender o código
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