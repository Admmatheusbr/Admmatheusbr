# Evidências técnicas das implementações

Verificação: 02/10/2026. Dados sintéticos, cópias isoladas.

## Gestão administrativa

3 testes unittest aprovados em 0.529s: backup antes da gravação; totais exatos, anulação e persistência; rejeição de entradas inválidas e datas futuras.

## Memória e busca semântica

6 testes pytest aprovados em 0.18s: operações de memória; ranking e limite; quatro cenários matemáticos de similaridade. Embeddings simulados. Não houve inferência real ou avaliação da qualidade de respostas.

## Versões examinadas

SHA-256 dos arquivos nas cópias usadas para a verificação. Permitem comparar versões numa avaliação autorizada; não substituem disponibilização de código ou nova execução.

| Arquivo | SHA-256 |
| --- | --- |
| Gestão: server.py | `21c692f824898314a29233d0082d6f6dd7fc4415541e605060e36f8590ac279a` |
| Gestão: test_ledger.py | `b31b89cb5b090b7f814dd68c205eb8eca094ba03256eaa4cb903ec976904d0de` |
| IA: memoria.py | `479fbf3fbd277457ff0b280b175b079b4378b8e962bff35c53f0163a15c93851` |
| IA: semantica.py | `cf27d7a6e6573fa04a4f34773bd78380d24cc50c3d9f20511884eed49f5a086c` |
| IA: test_memoria.py | `942c4c7ea64b419ccfa8eb52bd83c75f7148aad095a88580d9c53c9e421787eb` |

## Método e limites

As cópias vieram dos projetos existentes. Os testes de gestão usam banco temporário; os de memória substituem a base real por uma temporária e simulam embeddings. Nenhum banco real foi alterado. Foram usados unittest e pytest em um runtime Python disponível no ambiente de verificação.

O catálogo web foi examinado por leitura de código, sem execução nesta revisão. Os resultados não constituem auditoria integral de segurança, teste de produção ou medição de retorno financeiro.

## Exposição pública

Publicação documental: decisões e evidências selecionadas. Bancos reais, documentos privados, credenciais e código do núcleo local não estão incluídos. Uma avaliação adicional exige definir finalidade, acesso e material apropriado antes do compartilhamento.
