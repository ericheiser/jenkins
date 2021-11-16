# Habitat package: jenkins

[![IaC](https://app.soluble.cloud/api/v1/public/badges/a9bf6aca-cf4b-4612-a548-1d1736169dc0.svg)](https://app.soluble.cloud/repos/details/github.com/ericheiser/jenkins)  [![CIS](https://app.soluble.cloud/api/v1/public/badges/5ba0919f-2c32-41c8-a953-a22fdb9b3609.svg)](https://app.soluble.cloud/repos/details/github.com/ericheiser/jenkins)  [![HIPAA](https://app.soluble.cloud/api/v1/public/badges/79e60dcd-2f3d-4715-b5e2-0b9eecc5e576.svg)](https://app.soluble.cloud/repos/details/github.com/ericheiser/jenkins)  

[![Build Status](https://jmery-chef.visualstudio.com/Jenkins-Habitat/_apis/build/status/Jenkins-Habitat-CI?branchName=master)](https://jmery-chef.visualstudio.com/Jenkins-Habitat/_build/latest?definitionId=4?branchName=master)  [![Publish Status](https://jmery-chef.vsrm.visualstudio.com/_apis/public/Release/badge/e982e6c9-4110-4c47-b353-b04a162e73e0/1/1)](https://jmery-chef.visualstudio.com/Jenkins-Habitat/_release?view=mine&definitionId=1)

## Description

Build an run Jenkins preconfigured for CI/CD with habitat.

## Usage

`hab svc load jmery\jenkins`

See `default.toml` for default config values.

Includes a Terraform plan for AWS.  This will spin up the jenkins instance in aWS along with external DNS.   You must already have a TLD setup in Route53. Provide the zone name and zone id in your `terraform.tfvars` file.  See `example.tfvars`.
