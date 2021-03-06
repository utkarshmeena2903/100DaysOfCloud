# SEC02-AWS100 — Use a managed Config Rule

<p align="center" >
<img src="https://user-images.githubusercontent.com/69337392/176993657-adc28b7d-f48a-4525-b8f0-b8a766b9b86f.jpg" height="400" width="800" ></p>

## Introduction

✍️ Why?
- AWS Config currently supports the following managed rules in the analytics; compute; cryptography and PKI; database; machine learning; management and governance; migration and transfer; network and content delivery; security; identity and compliance; and storage categories

## Prerequisite

✍️ What?
- An AWS Config rule represents an AWS Lambda function that you create for a custom rule or a predefined function for an AWS Config managed rule. The function evaluates configuration items to assess whether your AWS resources comply with your desired configurations.
- AWS Config runs evaluation for the rule at a frequency that you specify, such as every 24 hours. Every 24 hours, the rule is triggered and AWS Config evaluates whether the passwords for your IAM users are compliant against the rule.

## Cloud Service Provider
- Amazon Web Services

## Difficulty
- Level 100 (Introductory)

## Estimated Time
1 hour

## Project's Author(s)
- [Andrew Brown](https://twitter.com/andrewbrown)

## Objectives

<p align="center" >
<img src="https://user-images.githubusercontent.com/69337392/176993678-f14bc679-7865-44c4-a6bc-64e8aefca999.png" height="400" width="700" ></p>

### You need to complete the following:

- Turn on AWS Config in the US-EAST-1 region
- Choose the managed Config rule eg. encrypted-volumes
- Launch an EC2 instance without an encryped EBS volume
- Monitor AWS Config until it detects there is an EBS volume that is unencrpyted

### You need to answer the following:

- What is AWS Config?
- What does an AWS Config rule do?
- What is remediation in the context of a config rule?

<p align="center" >
<img src="https://user-images.githubusercontent.com/69337392/176993670-faf0bc67-b94f-4488-acd3-6e4e77330d68.png" height="400" width="500" ></p>

## References

- [AWS Config](https://aws.amazon.com/config/)
