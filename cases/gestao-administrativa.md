# Gestão administrativa — controle local com histórico

**Contexto:** módulo existente do piloto MDu.World. Projeto próprio, desenvolvido com apoio de IA. Verificação em 02/10/2026 sobre cópia isolada, com dados sintéticos.

## Problema

Registros administrativos precisam manter valores exatos, rejeitar entradas inconsistentes e preservar a história quando um lançamento é anulado.

## Solução implementada

Módulo local de receitas e despesas com valores armazenados em centavos, validação de valor e data, persistência em SQLite, anulação preservando registros e backup antes das gravações.

## Resultado demonstrável

**3 testes aprovados:**

1. Totais exatos, anulação e persistência após reinicialização. O cenário passa de saldo de R$10,00 para -R$0,10 após anular a primeira receita, mantendo os três registros.
2. Rejeição de valores inválidos e datas futuras, sem criação de lançamentos.
3. Backup com o estado anterior à segunda gravação.

Esse resultado confirma os cenários testados; não mede economia de tempo e não equivale a conciliação bancária ou lucro contábil.

## Evidências

Fonte local: `mdu_app/server.py` e `mdu_app/test_ledger.py` do projeto existente. Relatório de verificação: [VERIFICACAO.md](../VERIFICACAO.md). O código e o banco privado não foram publicados nesta entrega.

## Aplicação comercial

Base para ferramentas internas de controle e revisão de registros, com escopo e regras acordados antes da implementação. Uma demonstração pode ser apresentada com dados fictícios.

**Tecnologias:** Python, SQLite, interface web local e testes automatizados.
