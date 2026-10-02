# Validação de dados cadastrais — CPF

**Contexto:** projeto acadêmico individual. Matheus Duarte confirmou que desenvolveu todo o trabalho. Código recuperado de materiais guardados pelo autor; não foi confirmada equivalência exata com a versão da gravação histórica.

## Problema
Cadastros precisam conferir entradas e comunicar inconsistências antes de seguir para outras etapas do processo.

## Solução
Aplicação de desktop em Python e Tkinter, com campo de entrada, botão e acionamento por Enter. A lógica confere quantidade de dígitos, sequências repetidas e dígitos verificadores. Há funções para registrar resultados em JSON e erros em log.

## Evidências
A gravação histórica mostra a interface e retorno de entrada inválida. Os três módulos recuperados tiveram sintaxe verificada. Em 02/10/2026, 11 cenários de entrada foram examinados em cópia isolada: 8 atenderam à política estrita proposta, e 3 mostraram normalização permissiva (letras, símbolos e dígitos Unicode). A GUI não foi executada nesta revisão.

## Resultado e limites
O case demonstra conexão entre interface, regras de validação e persistência. Não foi medido impacto comercial. A conferência matemática não comprova identidade, titularidade ou situação cadastral e não representa consulta oficial.

Antes de reutilizar: conferir formato antes de normalizar, rever dados completos nos registros e preservar arquivos com erro de leitura em vez de sobrescrevê-los. A aceitação de Unicode é uma decisão de contrato a definir. O código recuperado permanece privado nesta etapa, sem logs, dados ou vídeo no pacote público.

**Tecnologias:** Python, Tkinter, JSON e arquivos de log.
