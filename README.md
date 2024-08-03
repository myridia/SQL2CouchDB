# SQL2CouchDB
Migrate Sql queried Tables into CouchDb Documents

# Example
```sql
SELECT 
p.product_id
,p.model
,d.name
,d.description
,p.quantity
,p.image
,p.price
,p.status
,p.date_added 
FROM product as p
LEFT JOIN product_description AS d
On p.product_id = d.product_id
```


’’’

#How to compile it
```console
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
. "$HOME/.cargo/env"
```
