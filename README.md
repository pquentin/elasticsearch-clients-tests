# Serverless Clients Tests

This repository holds common tests for Elasticsearch Serverless Clients.

## Yaml tests

The tests are specified using the Elasticsearch YAML format reported [here](https://github.com/elastic/elasticsearch/blob/main/rest-api-spec/src/yamlRestTest/resources/rest-api-spec/test/README.asciidoc).

All the tests for serverless are located in the [tests](tests) folder. Each API endpoint has a folder
containing the tests to be executer. All the files must be executed in order and they are named
with a digit prefix.

**IMPORTANT:** the tests use a `test_serverless` index that must be delete before the execution of each test file.
