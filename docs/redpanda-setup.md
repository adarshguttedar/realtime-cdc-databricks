# Redpanda Cloud Setup

## Cluster
- Name: cdc-pipeline
- Type: Serverless free tier
- Region: Asia Mumbai ap-south-1
- Bootstrap server: seed-xxxx.xxxx.cloud.redpanda.com:9092

## Security
- User: debezium-user
- Protocol: SASL_SSL
- Mechanism: SCRAM-SHA-256

## Topics
- dbserver_prod.ecommerce.customers/products/orders/order_items/payments/shipping (3 partitions each)
- schema-changes.ecommerce_v3, connect-configs, connect-offsets, connect-statuses