# Biblioteca virtual — catálogo web

**Contexto:** protótipo acadêmico. Código existente no repositório [Site](https://github.com/Admmatheusbr/Site). Revisão de código em 02/10/2026.

## Problema

Um acervo precisa ser apresentado de forma organizada, permitindo navegar entre uma lista de livros e os detalhes de cada item.

## Solução implementada

Aplicação web com páginas de início, sobre, contato, catálogo e detalhes. As views renderizam templates e a página de detalhes seleciona um item pelo identificador recebido na rota. A lista é criada com cinco livros gerados para demonstração.

## Resultado demonstrável

O código reúne lista e detalhes em uma estrutura navegável e separa rotas, apresentação e geração dos dados. Isso demonstra organização básica de uma aplicação web. Não foi medido ganho de produtividade ou uso por clientes.

## Evidências

- [Views e seleção de livro](https://github.com/Admmatheusbr/Site/blob/main/biblioteca/views.py).
- [Rotas](https://github.com/Admmatheusbr/Site/blob/main/biblioteca/urls.py).
- [Templates](https://github.com/Admmatheusbr/Site/tree/main/biblioteca/templates/biblioteca).
- O arquivo de modelos da biblioteca não contém modelos de livros; o catálogo demonstrativo não é um cadastro persistente.

## Limites e próximos passos

O aplicativo não foi executado nesta revisão. Antes de oferecer uma versão para produção: validar execução em ambiente isolado, dependências e configuração, tratar itens inexistentes e definir cadastro persistente conforme o escopo. Não reutilizar o banco versionado como dados de demonstração pública sem revisão.

**Tecnologias:** Django, Python, templates HTML e Faker. Dependências históricas em `requisitos.txt`.
