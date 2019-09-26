# Local Lambda Kinesis Runner [![Build Status](https://travis-ci.org/kobybum/local-lambda-kinesis.svg?branch=master)](https://travis-ci.org/kobybum/local-lambda-kinesis)

A python utility for testing lambda kinesis handlers locally using real data.
At the time of writing, [AWS SAM](https://github.com/awslabs/serverless-application-model) supports running kinesis handlers locally on a custom event.
However, in many cases we would like to test the lambda handler on real data.

This utility reads from a kinesis stream, transforms the events and forwards them to the relevant handler.
