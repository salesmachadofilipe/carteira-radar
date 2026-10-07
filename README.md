# Radar da Carteira

Painel que lê os quatro relatórios operacionais em `.xlsx` — **Modelo de Servir**,
**Saúde do Cliente**, **Ruptura** e **Prospecção** — e monta os gráficos radar, os
rankings, a meta de captação do mês e a ficha por cliente.

## Usar

Abra a página publicada (GitHub Pages) ou o `index.html` local, e anexe cada
relatório no quadro correspondente. Se um arquivo for anexado no campo errado, a
página avisa qual relatório ele parece ser.

## O que cada bloco traz

- **Dados compilados** — índice geral do profissional, radar com todas as
  variáveis dos três relatórios de índice e busca por código de cliente.
- **Modelo de Servir** — aderência média por variável, 20 melhores e 20 piores,
  e as cinco listas de dias até o vencimento.
- **Saúde do Cliente** — pontuação média por variável, rankings e os valores
  brutos das cinco últimas colunas.
- **Ruptura** — incidência por variável, clientes em ruptura (6+ pontos),
  pontuação por cliente e meses acumulados.
- **Prospecção** — meta de captação do mês (3 clientes novos, 300K+, com
  Financial Planning executado e Fee Based), o funil que mostra onde se perde
  cada um, e a conferência de AuC, modelo de remuneração e Financial Planning
  contra os outros relatórios.

A Prospecção descreve a conta como foi aberta; os relatórios de índice descrevem
o estado atual. Conta nova costuma levar um ciclo para entrar nessas bases, então
"não consta" na conferência é situação esperada, não erro.

## Privacidade

Os `.xlsx` **não são enviados a lugar nenhum**. A leitura acontece inteiramente no
navegador (ZIP, XML e formatos de data lidos nativamente, sem biblioteca externa e
sem back-end). Este repositório contém apenas código — nenhum dado de cliente.

O `.gitignore` bloqueia planilhas por precaução: nunca versione relatório aqui.

## Requisitos

Navegador atual (Chrome, Edge ou Firefox). A descompactação usa `DecompressionStream`.
Sem servidor, sem build, sem dependências.
