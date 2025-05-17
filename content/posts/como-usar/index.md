---
title: Como usar Market2csv
date: 2025-04-25T19:14:41-03:00
draft: false
menu: Como usar
weight: 1
summary: " "
---

### Demo do funcionamento da ferramenta

![Como usar a ferramenta](como-usar.gif#center)

### Passo a passo

> **Consulte em <a href="{{< relref "posts/instalacao/index.md" >}}" target="_blank)">Instalação</a> como baixar e executar a ferramenta**

Ao abrir a ferramenta, será solicitado que você digite o que quer pesquisar nos marketplaces para realizar a extração dos dados:


![pesquisa](pesquisa.png#center)

Após a ferramenta identificar e mostrar a quantidade de anúncios encontrados, será solicitado quantos anúncios você quer analisar:
- Você pode digitar qualquer valor entre 1 ou a quantidade máxima de anúncios encontrados
    - Os anúncios são analisados por **ordem de relevância**. Exemplo:
    - Caso digite `10`, serão analisados os *10 primeiros resultados*
    - Anuncios patrocinados são considerados nesse ranking de relevância
- E caso queira **TODOS OS ANÚNCIOS ENCONTRADOS**, basta digitar `0 (zero)`:
    - Isso **levará um tempo** caso existam muitos resultados para a sua pesquisa, ou se for uma pesquisa mais genérica, como `camiseta branca` por exemplo, que retora mais de *60 mil anuncios*

![quantidade](quantidade.png#center)
> *Exemplo do funcionamento da ferramenta pesquisando por `celular xiaomi 5g`*


A ferramenta irá mostrar um texto informativo do progresso da extração dos dados dos anúncio, e caso aconteça algum problema na extração de algum dado, será mostrado também uma mensagem informativa.

E ao final, uma mensagem informando sobre a criação do arquivo `.csv` com os dados coletados e uma mensagem com o arquivo `.json` da ficha técnica completa de cada anúncio:

![final](final.png#center)



Coleta os seguintes dados em cada Marketplace:

```code
Mercado Livre:
    - Titulo
    - Condição: Novo, usado, recondicionado
    - Preço: Preço Base, Preço com desconto
    - Quantidade de Vendas
    - Estoque
    - Anuncio é patrocinado?
    - Anuncio está no Full?
    - Nota de avaliação
    - Quantidade de reviews
    - Link do anuncio
    - Nome do vendedor
    - Link da loja do vendedor
    - Tipo de loja do vendedor: (Padrão, Eshop, Loja Oficial)
    - Descrição
    - Ficha técnica completa do anúncio
```

*A extração de dados em outros marketplaces como Shopee, Amazon, Magalu estão em desenvolvimento e serão adicionados em atualizações futuras* 
