# Terraform-LinkedIn
LinkedIn learning course notes and scripts 

## WHAT IS TERRAFORM?

Check the documentation: https://www.terraform.io/intro/index.html

> Terraform is a tool for **building, changing, and versioning infrastructure safely and efficiently**. Terraform can manage **existing and popular service providers** as well as custom in-house solutions.

Configuration files **describe** to Terraform the **components needed** to run a single application or your entire datacenter.

Terraform generates an **execution plan** describing what it **will do** to reach the **desired state**, and then **executes it** to **build the described infrastructure**. As the **configuration changes**, Terraform is able to **determine what changed** and create **incremental execution plans** which can be **applied**.

The infrastructure Terraform can manage includes **low-level components such as compute instances, storage, and networking, as well as high-level components such as DNS entries, SaaS features, etc.**

Use cases: https://www.terraform.io/intro/use-cases.html

## WHAT IS IaC (Infrastructure as Code)?

> Infrastructure is **described using a high-level configuration syntax**. This allows a blueprint of your datacenter to be **versioned and treated** as you would any other **code**. Additionally, infrastructure can be **shared and re-used**.

## EXECUTION PLANS

Terraform has a **"planning" step** where it generates an execution plan. The execution plan shows what Terraform will do when you call **apply**. This lets you **avoid any surprises** when Terraform manipulates infrastructure.

## RESOURSE GRAPH 

Terraform builds a **graph of all your resources**, and parallelizes the creation and modification of any non-dependent resources. Because of this, Terraform builds infrastructure as **efficiently as possible**, and operators get insight into dependencies in their infrastructure.
