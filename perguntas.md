# Perguntas

## Aula 1

1 - Vimos no último vídeo uma funcionalidade interessante do GitHub: as issues. Com esta funcionalidade, podemos atingir alguns resultados interessantes na organização de um projeto.

Sobre o que podemos fazer com issues, avalie as afirmativas abaixo:

1) Podemos reportar problemas
2) Podemos sugerir melhorias no código
3) Podemos organizar quaisquer coisas que façam sentido para o projeto

- __As afirmativas 1, 2 e 3 estão corretas__

> Alternativa correta! Todas as afirmativas estão corretas, já que o propósito inicial das issues, como o nome já diz, era reportar e controlar os problemas e bugs de um projeto (afirmativa 1). Além disso, com o tempo, passaram a perceber que havia mais possibilidades nas issues, e elas foram utilizadas para sugestão de melhorias no projeto e pedidos de novas funcionalidades (afirmativa 2). Por fim, ótimos exemplos de usos das issues no GitHub são das comunidades PHPSP e PHPRio, que as utilizam para organizar os palestrantes e sugestões de palestras (afirmativa 3).

- Somente a afirmativa 2 está correta
- Somente as afirmativas 1 e 3 estão corretas
- Somente a afirmativa 3 está correta
- Somente as afirmativas 2 e 3 estão corretas
- Somente a afirmativa 1 está correta
- Somente as afirmativas 1 e 2 estão corretas

2 - Já vimos como sugerir melhorias ou reportar problemas utilizando issues, mas o nosso trabalho no mundo Open Source pode ser mais ativo. Através de pull requests, nós podemos enviar melhorias e correções para projetos.

Por que utilizar pull requests e não editar o projeto original?

- Para utilizar uma buzzword (pull request) legal0
- Para tirar o maior proveito da ferramenta (GitHub)
- __Para garantir a qualidade do projeto pelos seus líderes e organizadores__

> Alternativa correta! Através de pull requests, os principais mantenedores de um projeto podem analisar todas as alterações, aprová-las ou reprová-las, dar feedback e interagir de uma forma geral. Pull requests não são utilizados apenas para projetos Open Source. Muitas equipes utilizam pull requests em seu dia-a-dia, para enviar as alterações de código para revisão de algum supervisor.

3 - Tendo entendido o que são issues e pull requests, nada mais justo do que enviar um pull request para resolver uma issue, certo? Mas quando desenvolvemos, podemos realizar vários commits, o que pode não ser tão interessante para quem for revisar o pull request.

Por que é interessante unir os commits em um único para enviar um pull request?

- Para demonstrar domínio da ferramenta (Git)
- Para diminuir o log
- __Para que o responsável pela revisão do projeto tenha um único commit a revisar, com todas as alterações necessárias__

> Alternativa correta! Revisar um único commit é bem mais fácil e rápido do que analisar diversos commits que resolvem um problema em comum. Por isso, nestes casos, é interessante utilizar o git rebase -i.

## Aula 2

1 - No último vídeo, vimos como podemos trazer um único commit específico de outra branch para a branch em que estamos trabalhando.

Em que caso faz sentido trazer um commit específico para a branch atual?

- Quando queremos copiar o trabalho do colega
- __Quando um bug que afeta a branch atual já foi solucionado em outra branch__

> Alternativa correta! Se uma implementação é necessária em sua branch e já foi feita em outra branch, pode fazer sentido trazer um commit específico, utilizando o git cherry-pick.

- Quando queremos fazer o merge commit a commit

2 - No último vídeo, nós utilizamos o git bisect para encontrar determinado ponto na história do código em que alguma alteração foi introduzida. Fizemos isso, informando os estados do commit (se estava "bom" ou "ruim").

Para que o git bisect pode ser útil?

- Encontrar o culpado por um bug
- Para atualizar a nossa linha do tempo
- __Para encontrar o commit em que um bug foi introduzido__

> Alternativa correta! Encontrando o exato commit em que determinado bug foi introduzido, podemos revertê-lo ou até mesmo tentar entender o motivo daquele bug ter sido introduzido.

3 - Com o git blame, podemos ver quem é o responsável por cada linha no código.

Para que isso pode ser útil?

- __Para saber para quem perguntar sobre determinado bloco de código que não entendemos__

> Alternativa correta! Com o git blame, nós podemos saber quem é o responsável por determinada linha ou bloco de código que nós não entendemos, e com isso sabemos com quem tirar a dúvida!

- Para encontrar o culpado por um bug
- Para desfazer uma alteração

## Aula 3

1 - Durante o vídeo, nós visualizamos o nosso log de commits de uma forma um pouco mais visual, onde as diferentes branches são representadas por linhas separadas.

Qual o comando para exibir o log desta forma?

- git log
- __git log --graph__

> Alternativa correta! Desta forma, uma representação um pouco mais gráfica do log é exibida na linha de comando.

- git log --format

2 - Aprendemos de forma bem resumida sobre a estratégia de organização de branches, chamada Git Flow.

Quais as branches presentes nesta estratégia?

- __Master, Develop, Branches de feature, Branches de Hotfix e Branches de release__

> Alternativa correta! Cada uma das branches tem um propósito bem definido e nos ajudam a manter o nosso controle de versões bem organizado.

- Master e Develop
- Master, Ticket, Testing, Release

## Aula 4

1 - Vimos no último vídeo que o Git nos permite, através dos hooks, executar algum código quando determinado evento acontece.

Como podemos escrever um código que será executado em algum evento?

- Criando um código PHP e informando ao Git que o programa é um evento
- Criando um código Java e informando ao Git que o .jar gerado é um evento
- __Criando um arquivo Shell Script, onde seu nome representa o evento, dentro da pasta .git/hooks__

> Alternativa correta! Para ver com mais detalhes os possíveis hooks (eventos), confira este site: <https://githooks.com/>.

2 - Na última aula, vimos de forma bem rudimentar como configurar um processo de entrega contínua do nosso código.

Por que chamamos o resultado que alcançamos de entrega contínua?

- Porque estamos sempre entregando o código para o Git gerenciar
- Porque estamos constantemente entregando novas versões para o repositório remoto
- __Porque a cada commit (a cada mudança significativa na base de código), podemos fazer um push e entregar o sistema em produção__

> Alternativa correta! Entrega contínua é uma série de práticas que permitem que o código esteja de forma rápida e simples em produção. Tão rápido e simples quanto rodar um ```git push```. Para saber mais sobre o assunto, confira o curso [Integração Contínua: Maturidade e Produtividade no Desenvolvimento de Software](https://cursos.alura.com.br/course/integracao-continua-jenkins) aqui na Alura.
