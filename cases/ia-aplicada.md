# IA aplicada — memória organizada e busca semântica

**Contexto:** projeto próprio de IA local existente. Desenvolvimento com apoio de IA. Revisão e testes em cópia isolada em 02/10/2026.

## Problema

Informações dispersas dificultam localizar o contexto certo para responder uma consulta e manter uma base de conhecimento atualizada.

## Solução implementada

Armazenamento estruturado de conhecimento, com operações de criação, consulta, edição e exclusão. A camada semântica usa embeddings e similaridade de cosseno para ordenar os registros relevantes. A integração prevista no código consulta o Ollama local.

## Resultado demonstrável

**6 testes aprovados**, cobrindo persistência e atualização de conhecimento, ordenação e limite dos resultados e quatro cenários matemáticos de similaridade, incluindo vetores opostos e vetor nulo.

Os embeddings foram simulados. A aprovação verifica a lógica de memória e ranking; não comprova qualidade de respostas, disponibilidade do Ollama ou funcionamento integral offline.

## Evidências

Fonte local: `src/memoria.py`, `src/semantica.py` e `tests/test_memoria.py` do projeto existente. Relatório: [VERIFICACAO.md](../VERIFICACAO.md). Nenhum documento privado ou banco de conhecimento foi incluído na vitrine.

## Aplicação comercial

Base para assistentes internos e organização de documentação, começando por uma demonstração com conteúdo autorizado, perguntas de referência e avaliação de respostas.

**Tecnologias:** Python, SQLite, embeddings, similaridade de cosseno e integração Ollama.
