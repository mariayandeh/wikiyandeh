# Estoque

## Inventory \| Estoque

Estoque

| Campo | Descrição | Tipo | Restrições | Exemplo |
| :--- | :--- | :--- | :--- | :--- |
| store\_id\* | Identificador interno da loja | integer ou string | -- | 1 |
| sku\* | Código de barras \(EAN 13 ou DUN14\) quando o mesmo possuir | string | Tamanho máximo de 20 caracteres | "11402329312324” |
| quantity\* | Quantidade do produto em estoque | float | -- | 3.0 |
| is\_in\_stock | Indica se o produto está em estoque ou esgotado | boolean | true/false ou 0/1 | true |
| manage\_stock | Indica se o estoque deste produto será gerenciável | boolean | true/false ou 0/1 | true |

 \* Campos obrigatórios

## 

### Exemplo de consulta em SQL:

```sql
SELECT store_id     AS "store_id", 
       sku          AS "sku", 
       is_in_stock  AS "is_in_stock", 
       manage_stock AS "manage_stock", 
       quantity     AS "quantity" 
FROM   view_inventory 
```

