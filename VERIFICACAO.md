# Evidências de testes — 02/10/2026

Executados em cópias isoladas dos projetos existentes, com dados sintéticos.

## Gestão administrativa

```text
test_backup_contains_pre_write_state ... ok
test_exact_totals_void_and_persistence ... ok
test_reject_invalid_money_and_future ... ok
Ran 3 tests in 0.529s
OK
```

## Memória e busca semântica

```text
tests/test_memoria.py
...... [100%]
6 passed in 0.18s
```

Embeddings simulados pelo teste; não foi executada inferência real. O runtime antigo não iniciou. A execução aprovada usou o runtime Python do Codex, as bibliotecas já existentes e uma pasta temporária no workspace.

Não houve alteração dos bancos reais dos projetos.

