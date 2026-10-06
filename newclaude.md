# NewClaude

App desktop de IA para Windows, local-first, que reúne vários modelos de linguagem num só lugar e vai orquestrar mais de um agente na mesma tarefa.

Em desenvolvimento. Código privado.

## Objetivo

Uma estação de trabalho no estilo do Claude Desktop que converse com vários provedores de modelo, guarde tudo na máquina e execute comandos e edições de arquivo com controle de risco.

## O que já funciona

- Conversa com vários provedores, com resposta em streaming.
- Banco local SQLite com 21 tabelas e migrações versionadas, usando o SQLite nativo do Node 22.
- Isolamento do Electron (contextIsolation, preload, bloqueio de navegação) e acesso a arquivos restrito às pastas autorizadas.
- Classificador de risco para comandos de terminal e detector de loop para agentes.
- Terminal real com node-pty e visualizador de diff.
- Chaves de API guardadas no Gerenciador de Credenciais do Windows.

## Próximos passos

Ligar o cliente MCP, o fluxo de aprovação para escrita em arquivo e terminal, e a orquestração de vários agentes. Essas partes já têm interface, mas ainda não têm backend.

## Stack

Electron 36, React 19, TypeScript, Vite, Tailwind CSS 4, node:sqlite, keytar, node-pty, Vitest.
