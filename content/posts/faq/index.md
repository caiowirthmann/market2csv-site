---
title: "FAQ e Suporte"
date: 2025-04-25T23:14:41-03:00
draft: false
weight: 5
menu: FAQ e Suporte
summary: " "
---

Se você tiver **dúvidas, sugestões**, encontrar algum **problema**, quiser contribuir com o projeto ou quiser solicitar **customização** da ferramenta em específico, entre em contato pelos canais abaixo:

## Contato

- **Telegram:** [@caiowp](https://t.me/caiowp)  
- **Discord:** [musaaaa4](https://discord.com/users/279083512638734336)  
- **Github** [caiowirthmann](https://github.com/caiowirthmann/)
- **Link do código do projeto** [Market2csv](https://github.com/caiowirthmann/market2csv)

---

##  Perguntas Frequentes (FAQ)

###  O CSV abre de forma estranha ou mal formatado no Excel, Google Sheets, LibreOffice. O que faço?

O CSV gerado pela ferramenta usa `;` (ponto e virgula) como o delimitador padrão das colunas. Ao abrir ou importar o CSV para o editor de planilhas, verifique se está sendo usado o delimitador correto.

Verifique também se o **delimitador de texto** está configurado para `"` (aspas).

<br>

###  Um campo do CSV está vazio. O que aconteceu?

Pode ocorrer algum erro durante a extração dos dados ou o marketplace realizar alguma alteração na forma/localização onde o dado é alterado e isso impactar na extração do dado.

Em casos de erro, é gerado um log com uma mensagem detalhada do erro que aconteceu e dados para identificar em qual anúncio aconteceu, e o campo no csv é preenchido com um valor "neutro"

<br>


###  A ferramenta parou de funcionar ou está dando erro. E agora?

Isso pode acontecer por mudanças no layout do marketplace, alguma instabilidade no site ou problemas na conexão.

Casos de alteração de layout que acarretam em erro na extração dos dados geram um log também.

Verifique sua conexão e os logs que são gerados, tente novamente mais tarde ou entre em contato.

Existe também uma consideração técnica que ferramentas de extração de dados (scraper, web-crawlers e outros) podem encontrar e resultar em erros (erro 429, rate-limit, entre outros):

- Sites em sua grande maioria possuem configurações e restrições de quantos "requests" um mesmo usuário, IP pode fazer para o servidor antes de limitar ou barrar a conexão. Por conta disso e motivos éticos, scrapers/web-crawlers adicionam intervalos e outras técnicas nos "requests" para que funcione dentro dos requisitos de cada site

- Market2csv já vem com essas configurações e medidas prontas, não é necessária configuraçãoa adicional. Caso queira e tenha o conhecimento técnico, você pode verificar o código-fonte e realizar as suas alterações

<br>

###  Qual o limite de anúncios que posso baixar de uma vez?

A ferramenta permite definir a quantidade que quiser e pode-se executar quantas vezes quiser. É valido citar que quanto mais anúncios você solicitar para coletar os dados, mais tempo levará

<br>

###  Posso usar essa ferramenta para outro país (ex: Mercado Libre Argentina)?

Atualmente a ferramenta funciona somente para versões **brasileiras** (ex: Mercado Livre Brasil (MLB)) independente da sua localização.

<br>


