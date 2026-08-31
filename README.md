# Radar da Carteira

Painel que lê os três relatórios operacionais em `.xlsx` — **Modelo de Servir**,
**Saúde do Cliente** e **Ruptura** — e monta os gráficos radar, os rankings e a
ficha por cliente.

## Usar

Abra a página publicada (GitHub Pages) ou o `index.html` local, e anexe cada
relatório no quadro correspondente. Se um arquivo for anexado no campo errado, a
página avisa qual relatório ele parece ser.

## Privacidade

Os `.xlsx` **não são enviados a lugar nenhum**. A leitura acontece inteiramente no
navegador (ZIP + XML nativos, sem biblioteca externa e sem back-end). Este
repositório contém apenas código — nenhum dado de cliente.

O `.gitignore` bloqueia planilhas por precaução: nunca versione relatório aqui.

## Requisitos

Navegador atual (Chrome, Edge ou Firefox). A descompactação usa `DecompressionStream`.
Sem servidor, sem build, sem dependências.
