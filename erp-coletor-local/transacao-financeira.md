---
description: Modelo de dados finantial-transaction | Transação Financeira
---

# Transação Financeira

Transação Financeira

| Campo | Descrição | Tipo |
| :--- | :---: | ---: |
| **transaction\_id\*** | **Identificador da transação** |  **string** |
| **ccflag\_id\*** | **Código da bandeira** | **string** |
| **operation\_id\*** | **Código da operação financeira** | **string** |
| **sales\_date\*** | **data da venda** | **string** |
| payment\_store\_date | data de pagamento da loja | string |
| **sales\_value\*** | **valor da venda** | **number** |
| discount\_value | valor do desconto | number |
| store\_value | valor a pagar da loja | number |
| **transaction\_status\*** | **status da transação \(approved, denied, undone\)** | **string** |
| **payment\_status\*** | **Status do pagamento \(retained, effected, rejected\)** | **string** |
| nsu | NSU | string |
| original\_nsu | NSU Original | string |
| installments | Número das parcelas | number |
| pos | POS | string |
| authorization | Autorização da transação | string |
| bin | BIN | string |
| tax | Taxa \(exemplo: 7.5\) | number |
| tid\_number | número do TID | string |
| mid\_number | número do MID | string |
| capture\_type | Tipo de captura \(POS, TEF, Ecommerce\) | string |
| equipment\_model | Modelo do equipamento | string |
| chip\_type | tipo do chip | string |

