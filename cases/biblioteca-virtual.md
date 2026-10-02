# MDu EntreVozes — biblioteca demonstrativa

**Identidade:** nome fictício e provisório vinculado à MDu.World. A demonstração não representa uma entrega ou parceria com a instituição originalmente citada. Recursos de audiobooks e acessibilidade ainda não fazem parte da implementação examinada.

**Contexto:** estudo acadêmico. Revisão de código em 02/10/2026. A vitrine pública apresenta a implementação examinada e seu alcance.

## Problema

Um acervo precisa ser apresentado de forma organizada, permitindo navegar entre uma lista de livros e os detalhes de cada item.

## Solução implementada

Aplicação web com páginas de início, sobre, contato, catálogo e detalhes. As views renderizam templates e a página de detalhes seleciona um item pelo identificador recebido na rota. A lista é criada com cinco livros gerados para demonstração.

## Resultado demonstrável

O código reúne lista e detalhes em uma estrutura navegável e separa rotas, apresentação e geração dos dados. Isso demonstra organização básica de uma aplicação web. Não foi medido ganho de produtividade ou uso por clientes.

## Evidências

- Views com geração da lista e seleção do livro pelo identificador.
- Rotas de catálogo e detalhes definidas.
- Templates separados por páginas e parciais.
- O arquivo de modelos da biblioteca não contém modelos de livros; o catálogo demonstrativo não é um cadastro persistente.

## Limites e próximos passos

O aplicativo não foi executado nesta revisão. Antes de oferecer uma versão para produção: validar execução em ambiente isolado, dependências e configuração, tratar itens inexistentes e definir cadastro persistente conforme o escopo. Não reutilizar o banco versionado como dados de demonstração pública sem revisão.

**Tecnologias:** Django, Python, templates HTML e Faker. Dependências históricas em `requisitos.txt`.

## Decisões e maturidade

Separar rotas, views e templates organiza responsabilidades. Os dados gerados tornam o catálogo demonstrativo, sem comprovar persistência. O tratamento de item inexistente e a revisão de dependências são próximos passos, não funcionalidades atribuídas à entrega atual.

O repositório acadêmico legado precisa de revisão de configuração e banco versionado antes de voltar a ser destacado com acesso direto ao código. Materiais de terceiros utilizados na formação não são apresentados como autoria exclusiva.

