---
title: "Limitações"
date: 2025-04-25T22:14:41-03:00
draft: false
weight: 4
summary: "Limitações da ferramenta em cada marletplace"
---

# Limitações da ferramenta nos marketplaces


## Mercado Livre

Algumas informações exibidas nos anúncios do Mercado Livre são disponibilizadas de forma limitada ou não-exatas (principalmente por questões de privacidade implementadas pelo Mercado Livre). Abaixo segue a explicação para cada campo em que isso acontece:

### Quantidade de vendas

O número de vendas exibido nos anúncios do Mercado Livre segue um padrão de **faixas** após 5 unidades vendidas. Então:

- Anuncios com até 5 unidades, o número exato é mostrado.
- Após isso (5+ vendas), o site exibe apenas pelo **PRIMEIRO VALOR** de um **INTERVALO APROXIMADO**

```code
5 a 9 - Exibido como +5 Vendidos
10 a 24 - Exibido como +10 Vendidos
25 a 49 - Exibido como +25 Vendidos
50 a 99 - Exibido como +50 Vendidos
100 a 499 - Exibido como +100 Vendidos
500 a 999 - Exibido como +500 Vendidos

A partir de 1000 unidades vendidas começa a aparece "mil" de forma literal ao invés de "000"

1000 a 4.999 - Exibido como +1000 Vendidos
5mil a 9.999 - Exibido como +5mil Vendidos
10mil a 49.999 - Exibido como +10mil Vendidos
50mil a 99.999 - Exibido como +50mil Vendidos
+100mil - Exibido como +100mil Vendidos
```
### Estoque

Situação similar a quantidade de vendas, o numero **EXATO** é disponibilizado somente até **5 unidades**, após isso é disponibilizado em **faixas**

> Caso o anúncio não tenha estoque (0 unidades), o anúncio fica pausado e só é possível acessá-lo se tiver o link dele. Ele não aparece na busca


```code
1 - Último disponível!
5 a 9 - +5 disponíveis
10 a 24 - +10 disponíveis
25 a 49 - +25 disponíveis
50 a ... - +50 disponíveis
```

*Apesar do mercado livre não disponibilizar uma forma de acessar a quantidade de estoque disponível no anúncio, existem meios de descobrir o número exato.<br>É necessário que o vendedor não tenha definido um limite de unidades por compra no anúncio (na opção de quantidade aparece um menu com a opção `mais de x unidades`) e que você tenha tempo de sobra. Basta clicar na opção e ir mudando para um valor que não aparece a mensagem de "sem estoque" quando você digitar o valor. Tentativa e erro, bateção de lata*

### Frete (Envios Full, Flex)

Frete ***por enquanto*** não é uma opção disponibilizada na ferramenta:

- Calculo do frete é multifatorial:
    - Categoria do anúncio
    - Reputação do vendedor
    - Valor de venda do anúncio
    - Dimensões do produto
    - Forma de entrega
    - Região despacho x Região entrega


> O valor de frete é calculado e mostrado no anúncio quando se está **logado** na sua conta do mercado livre, e for selecionada a forma de entrega <mark>Mercado Envios, Full e Mercado Envios Flex</mark> e o endereço de entrega (é possível ter mais de um endereço de entrega, mas na conta você seleciona um "padrão" que será usado para esses calculos e mostrado primeiro)

A coluna de `Full` da ferramenta mostra apenas se o anúncio tem Mercado Envios Full ou não. O valor em sí segue a mesma questão citada acima

---

## Shopee

*Em construção*

---

## Amazon

*Em construção*

---

## Magalu

*Em construção*