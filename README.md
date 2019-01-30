## To create a Kafka Cluster run the below to a kafka namespace
`helm install --name kafka -f ./kafka/values.yml incubator/kafka --tls`

## To install the schema-registry use this (do not use schema-registry as service name)
`helm install --name sr incubator/schema-registry -f values.yml --tls`

## To install the Kafka-connect run the below
`helm install --name kc confluent/charts/cp-kafka-connect -f values --tls`