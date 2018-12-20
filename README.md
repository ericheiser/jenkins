# Habitat package: jenkins

[![Build Status](https://jmery-chef.visualstudio.com/Jenkins-Habitat/_apis/build/status/Jenkins-Habitat-CI?branchName=master)](https://jmery-chef.visualstudio.com/Jenkins-Habitat/_build/latest?definitionId=4?branchName=master)  [![Publish Status](https://jmery-chef.vsrm.visualstudio.com/_apis/public/Release/badge/e982e6c9-4110-4c47-b353-b04a162e73e0/1/1)](https://jmery-chef.visualstudio.com/Jenkins-Habitat/_release?view=mine&definitionId=1)

## Description

Build an run Jenkins preconfigured for CI/CD with habitat.

## Usage

`hab svc load jmery\jenkins`

See `default.toml` for default config values.

Includes a Terraform plan for AWS.  This will spin up the jenkins instance in aWS along with external DNS.   You must already have a TLD setup in Route53. Provide the zone name and zone id in your `terraform.tfvars` file.  See `example.tfvars`.
