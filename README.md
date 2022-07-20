# DevOps 技術分享 Miguel
## IaC coding 
### Goal
* extensibility: how to create a new project quickly and exactly?
* changeability: how faster if you wanna update to all project?
* readability: distinct responsibility via directory and file.

### practices sharing 
* terraform
```
<buisness>
|-gcp
  |-- modules
     |-- computer_instance
       |-- main.tf
       |-- variables.tf
       |-- output.tf
     |-- office_firewall
  |-- <gcp project/ customer>
     |-- terraform.tfstate
     |-- computer_instance.tf
     |-- container_cluster.tf
     |-- provider.tf
     |-- output.tf
     |-- variables.tf
          |-- project, region, name, preemptible, node_count etc.
|-aws
```

### Improvement
* Inheritance and override.
* Follow standard conventions. 
* How/When to Refactor.

## Coding Quality  
* Test is it works before push
* Review PR by yourself first
* Record Steps clearly during development
* Everybody's code should be review

## CI
* [static test](https://blogs.perficient.com/2021/09/22/utilizing-static-analysis-testing-for-infrastructure-as-code/)
* integration test

## CD/GitOps
* [argocd](https://www.youtube.com/watch?v=aWDIQMbp1cc&t=64s)
* AWX
* Terraform cloud
* [apollo config](https://www.apolloconfig.com/#/zh/README)

