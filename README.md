# Serverless Clients Tests

This repository holds common tests for Elasticsearch Serverless Clients.

## Yaml tests

The tests are specified using the Elasticsearch YAML format reported [here](https://github.com/elastic/elasticsearch/blob/main/rest-api-spec/src/yamlRestTest/resources/rest-api-spec/test/README.asciidoc).

All the tests for serverless are located in the [tests](tests) folder. Each API endpoint has a folder
containing the tests to be executer. All the files must be executed in order, they are enumerated with
a digit prefix.

To speed up the tests, we used a naming convention to use a different index name for each test.
This means we do not need to execute a cleanup phase after each test. You can remove all the indexes
at the end of execution of all the tests, using the [DELETE index](https://www.elastic.co/guide/en/elasticsearch/reference/current/indices-delete-index.html)
API with the `*` wildcard.