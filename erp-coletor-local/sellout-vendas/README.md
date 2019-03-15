---
description: Modelo de Dados - "SellOut" | Vendas para Clientes
---

# Sellout \(Vendas\)

| A entidade Sellout  tem como registros cada uma das vendas realizadas para os clientes. Estando preparada para descrever cada um dos seguintes tipos fiscais: ECF, CF-e, NF-e e NFC-e. |
| :--- |


## SellOut   <a id="sellin---itens"></a>

| Campo | Descrição | Tipo | Restrições | Exemplo |
| :--- | :--- | :--- | :--- | :--- |


| <table>
  <thead>
    <tr>
      <th style="text-align:left">Campo</th>
      <th style="text-align:left">Descri&#xE7;&#xE3;o</th>
      <th style="text-align:left">Tipo</th>
      <th style="text-align:left">Restri&#xE7;&#xF5;es</th>
      <th style="text-align:left">Exemplo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">store\_id\* | Identificador interno da loja | integer ou string | -- | 1 |
| :--- | :--- | :--- | :--- | :--- |


| id\* | Identificador da venda | string | *</td>
      <td style="text-align:left">Identificador interno da loja</td>
      <td style="text-align:left">integer ou string</td>
      <td style="text-align:left">--</td>
      <td style="text-align:left">1</td>
    </tr>
    <tr>
      <td style="text-align:left">id*</td>
      <td style="text-align:left">Identificador da venda</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">tamanho má&#xE1;ximo de 50 caracteres | “RCNTH345987” |
| :--- | :--- | :--- | :--- | :--- |


| </td>
      <td style="text-align:left">&#x201C;RCNTH345987&#x201D;</td>
    </tr>
    <tr>
      <td style="text-align:left">sellout\_timestamp\* | Data e hora da venda | string | satisfazer o padrão “YYYY-MM-DDTHH:MM:SS” | “2017-08-20T14:55:08” |
| :--- | :--- | :--- | :--- | :--- |


| *</td>
      <td style="text-align:left">Data e hora da venda</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">satisfazer o padr&#xE3;o &#x201C;YYYY-MM-DDTHH:MM:SS&#x201D;</td>
      <td style="text-align:left">&#x201C;2017-08-20T14:55:08&#x201D;</td>
    </tr>
    <tr>
      <td style="text-align:left">nome\_operador | Nome do operador do PDV | string | -- | “Maria Cristina” |
| :--- | :--- | :--- | :--- | :--- |


| </td>
      <td style="text-align:left">Nome do operador do PDV</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">--</td>
      <td style="text-align:left">&#x201C;Maria Cristina&#x201D;</td>
    </tr>
    <tr>
      <td style="text-align:left">nome\_vendedor | Nome do vendedor | string | -- | “Ana Maria” |
| :--- | :--- | :--- | :--- | :--- |


| </td>
      <td style="text-align:left">Nome do vendedor</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">--</td>
      <td style="text-align:left">&#x201C;Ana Maria&#x201D;</td>
    </tr>
    <tr>
      <td style="text-align:left">store\_taxpayer\_id\* | CNPJ da loja que realizou a venda | string | tamanho exato de 14 caracteres | “05345647000122” |
| :--- | :--- | :--- | :--- | :--- |


| *</td>
      <td style="text-align:left">CNPJ da loja que realizou a venda</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">tamanho exato de 14 caracteres</td>
      <td style="text-align:left">&#x201C;05345647000122&#x201D;</td>
    </tr>
    <tr>
      <td style="text-align:left">buyer\_taxpayer\_id | CPF ou CNPJ do comprador final | string | tamanho exato de 11 ou 14 caracteres | “83230677323” |
| :--- | :--- | :--- | :--- | :--- |


| </td>
      <td style="text-align:left">CPF ou CNPJ do comprador final</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">tamanho exato de 11 ou 14 caracteres</td>
      <td style="text-align:left">&#x201C;83230677323&#x201D;</td>
    </tr>
    <tr>
      <td style="text-align:left">checkout\_id | Identificador do ponto de venda | string | -- | “2938923” |
| :--- | :--- | :--- | :--- | :--- |


| </td>
      <td style="text-align:left">Identificador do ponto de venda</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">--</td>
      <td style="text-align:left">&#x201C;2938923&#x201D;</td>
    </tr>
    <tr>
      <td style="text-align:left">receipt\_number | Nú</td>
      <td style="text-align:left">N&#xFA;mero do documento fiscal \(NF-e/NFC-e/CF-e\) | string | )</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">tamanho má&#xE1;ximo de 50 caracteres | “33093” |
| :--- | :--- | :--- | :--- | :--- |


| </td>
      <td style="text-align:left">&#x201C;33093&#x201D;</td>
    </tr>
    <tr>
      <td style="text-align:left">receipt\_series\_number | Sé</td>
      <td style="text-align:left">S&#xE9;rie do documento fiscal \(NF-e/NFC-e/CF-e\) ou CCF \(ECF\) | string | )</td>
      <td
      style="text-align:left">string</td>
        <td style="text-align:left">No caso de documento ECF, obrigató&#xF3;rio informar o CCF neste campo | “27” |
| :--- | :--- | :--- | :--- | :--- |


| coo | Nú</td>
        <td
        style="text-align:left">&#x201C;27&#x201D;</td>
    </tr>
    <tr>
      <td style="text-align:left">coo</td>
      <td style="text-align:left">N&#xFA;mero do COO \(ECF\) | string | )</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">Campo obrigató&#xF3;rio para documentos tipo ECF | “123742” |
| :--- | :--- | :--- | :--- | :--- |


<table>
  <thead</td>
      <td style="text-align:left">&#x201C;123742&#x201D;</td>
    </tr>
    <tr>
      <thd style="text-align:left">nfe_access_key</thd>
      <thd style="text-align:left">Chave do documento NFC-e/CF-e associado &#xE0; venda</thd>
      <thd style="text-align:left">string</thd>
      <thd style="text-align:left">Satisfazer o padr&#xE3;o exato de come&#xE7;ar com 3 caracteres de tipo
        (&#x201C;NFe&#x201D; ou &#x201C;CFe&#x201D;) seguido por 44 caracteres
        num&#xE9;ricos</thd>
      <thd style="text-align:left">
        <p>NFCe:&#x201C;NFe31170901704848000164650020000018481058491134&#x201D; ou</p>
        <p>CF-e: &#x201C;CFe35150310860014000139590010000162181020002180&#x201D;;</p>
      </thd>
    </tr>
  </thead>
  <tbody></tbody>
</table>|   <tr>
      <td style="text-align:left">device\_id | Número do dispositivo | string | </td>
      <td style="text-align:left">N&#xFA;mero do dispositivo</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">Deve sempre ser fornecido para documentos do tipo ECF e em forma completa
        \(em vez de reduzida\). **<b>Tamanho má&#xE1;ximo de 50 caracteres** | “BE1000199329329922” |
| :--- | :--- | :--- | :--- | :--- |


| </b>
      </td>
      <td style="text-align:left">&#x201C;BE1000199329329922&#x201D;</td>
    </tr>
    <tr>
      <td style="text-align:left">seller\_id | </td>
      <td style="text-align:left">CPF do vendedor associado a esta, caso exista vendedor relacionado | string | tamanho exato de 11 caracteres | “83230677323” |
| :--- | :--- | :--- | :--- | :--- |


| </td>
      <td
      style="text-align:left">string</td>
        <td style="text-align:left">tamanho exato de 11 caracteres</td>
        <td style="text-align:left">&#x201C;83230677323&#x201D;</td>
    </tr>
    <tr>
      <td style="text-align:left">sales\_addition\* | *</td>
      <td style="text-align:left">Valor de acré&#xE9;scimo na venda | float | -- | 0.50 |
| :--- | :--- | :--- | :--- | :--- |


| sales\_discount\* | Valor de desconto na venda | float | -- | 1.75 |
| :--- | :--- | :--- | :--- | :--- |


| subtotal\* | Valor do subtotal da venda | float | -- | 5.93 |
| :--- | :--- | :--- | :--- | :--- |


<table>
  <thead</td>
      <td style="text-align:left">float</td>
      <td style="text-align:left">--</td>
      <td style="text-align:left">0.50</td>
    </tr>
    <tr>
      <td style="text-align:left">sales_discount*</td>
      <td style="text-align:left">Valor de desconto na venda</td>
      <td style="text-align:left">float</td>
      <td style="text-align:left">--</td>
      <td style="text-align:left">1.75</td>
    </tr>
    <tr>
      <td style="text-align:left">subtotal*</td>
      <td style="text-align:left">Valor do subtotal da venda</td>
      <td style="text-align:left">float</td>
      <td style="text-align:left">--</td>
      <td style="text-align:left">5.93</td>
    </tr>
    <tr>
      <thd style="text-align:left">cancellation_flag*</thd>
      <thd style="text-align:left">Indica se a venda foi cancelada ou n&#xE3;o</thd>
      <thd style="text-align:left">string</thd>
      <thd style="text-align:left">
        <p>limita-se apenas aos valores:</p>
        <p>&#x25CF; &#x201C;N&#x201D; : venda n&#xE3;o-cancelada &#x25CF; &#x201C;S&#x201D;
          : venda cancelada</p>
      </thd>
      <thd style="text-align:left">&#x201C;N&#x201D;</thd>
    </tr>
  </thead>
  <tbody></tbody>
</table><table>
  <thead>
    <tr>
      <thd style="text-align:left">operation</thd>
      <thd style="text-align:left">Tipo da opera&#xE7;&#xE3;o realizada</thd>
      <thd style="text-align:left">string</thd>
      <thd style="text-align:left">
        <p>limita-se apenas aos valores:</p>
        <p>&#x25CF; &#x201C;E&#x201D; : entrada</p>
        <p>&#x25CF; &#x201C;S&#x201D; : sa&#xED;da</p>
        <p>&#x25CF; &#x201C;DE&#x201D; : devolu&#xE7;&#xE3;o de entrada</p>
        <p>&#x25CF; &#x201C;DS&#x201D; : devolu&#xE7;&#xE3;o de sa&#xED;da</p>
        <p>&#x25CF; &#x201C;N&#x201D; : neutro</p>
        <p>&#x25CF; &#x201C;NULL&#x201D; : n&#xE3;o dispon&#xED;vel</p>
      </thd>
      <thd style="text-align:left">&#x201C;E&#x201D;</thd>
    </tr>
  </thead>
  <tbody></tbody>
</table><table>
  <thead>
    <tr>
      <thd style="text-align:left">transaction_type</thd>
      <thd style="text-align:left">Indica qual tipo de transa&#xE7;&#xE3;o realizada</thd>
      <thd style="text-align:left">string</thd>
      <thd style="text-align:left">
        <p>limita-se apenas aos valores:</p>
        <p>&#x25CF; &#x201C;J&#x201D; : ajuste de estoque</p>
        <p>&#x25CF; &#x201C;P&#x201D; : faturamento de pedido</p>
        <p>&#x25CF; &#x201C;S&#x201D; : normal</p>
        <p>&#x25CF; &#x201C;E&#x201D; : entrada</p>
        <p>&#x25CF; &#x201C;D&#x201D; : transfer&#xEA;ncia entre dep&#xF3;sitos</p>
        <p>&#x25CF; &#x201C;T&#x201D; : transfer&#xEA;ncia</p>
      </thd>
      <thd style="text-align:left">&quot;P&quot;</thd>
    </tr>
  </thead>
  <tbody></tbody>
</table>| ipi | Valor do IPI sobre a venda | float | -- | 1.87 |
| :--- | :--- | :--- | :--- | :--- |


| iss | Valor do ISS sobre a venda | float | -- | 1.01 |
| :--- | :--- | :--- | :--- | :--- |


| frete | Valor de frete da venda | float | -- | 25.98 |
| :--- | :--- | :--- | :--- | :--- |


<table>
  <thead  <tr>
      <td style="text-align:left">ipi</td>
      <td style="text-align:left">Valor do IPI sobre a venda</td>
      <td style="text-align:left">float</td>
      <td style="text-align:left">--</td>
      <td style="text-align:left">1.87</td>
    </tr>
    <tr>
      <td style="text-align:left">iss</td>
      <td style="text-align:left">Valor do ISS sobre a venda</td>
      <td style="text-align:left">float</td>
      <td style="text-align:left">--</td>
      <td style="text-align:left">1.01</td>
    </tr>
    <tr>
      <td style="text-align:left">frete</td>
      <td style="text-align:left">Valor de frete da venda</td>
      <td style="text-align:left">float</td>
      <td style="text-align:left">--</td>
      <td style="text-align:left">25.98</td>
    </tr>
    <tr>
      <thd style="text-align:left">tipo</thd>
      <thd style="text-align:left">Indica qual tipo de documento fiscal</thd>
      <thd style="text-align:left">string</thd>
      <thd style="text-align:left">
        <p>limita-se apenas aos valores:</p>
        <p>&#x25CF; &#x201C;ecf&#x201D; : SPED Fiscal</p>
        <p>&#x25CF; &#x201C;nfce&#x201D; : Nota Fiscal de Consumidor Eletr&#xF4;nica</p>
        <p>&#x25CF; &#x201C;sat&#x201D; : SAT Fiscal</p>
        <p>&#x25CF; &#x201C;nfe&#x201D; : Nota Fiscal Eletr&#xF4;nica</p>
      </thd>
      <thd style="text-align:left">&#x201C;nfce&#x201D;</thd>
    </tr>
  </thead>
  <tbody>
</tbody>
</table>able>### Exemplo da consulta em SQL:

```text
SELECT store_id              AS "store_id", 
       sellout_timestamp     AS "sellout_timestamp", 
       id                    AS "id", 
       nome_operador         AS "nome_operador", 
       nome_vendedor         AS "nome_vendedor", 
       store_taxpayer_id     AS "store_taxpayer_id", 
       buyer_taxpayer_id     AS "buyer_taxpayer_id", 
       checkout_id           AS "checkout_id", 
       receipt_number        AS "receipt_number", 
       receipt_series_number AS "receipt_series_number", 
       coo                   AS "coo", 
       nfe_access_key        AS "nfe_access_key", 
       device_id             AS "device_id", 
       seller_id             AS "seller_id", 
       sales_addition        AS "sales_addition", 
       sales_discount        AS "sales_discount", 
       subtotal              AS "subtotal", 
       cancellaion_flag      AS "cancellaion_flag", 
       operation             AS "operation", 
       transaction_type      AS "transaction_type", 
       ipi                   AS "ipi", 
       iss                   AS "iss", 
       frete                 AS "frete", 
       tipo                  AS "tipo" 
FROM   view_sellout
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbNzY2OTA3ODE3XX0=
-->