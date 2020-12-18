# Lab 4: Publishing a VM Offer

## Introduction

*Virtual Machine offers* are used to deploy and transact a virtual machine (VM) instance through Marketplace. The solution must consist of a single VM. Anything more complex requires an *Azure Apps offer*.

When a customer 'purchases' a *VM offer*, the VM will be deployed into the customer's Azure subscription. As a consequence, VM offers can only be published in *Azure Marketplace* (not *AppSource*).

*VM offers* support the *Transact* listing type. They also support the *BYOL* listing type (and, by offering limited time licences via a *BYOL* listing, they also support free trials). A *Test drive* option is also available.

Transact *VM offers* are billed on a usage-based PAYG (Pay As You Go) model. Each plan can be created with a free trial option giving you the option to offer customers a 1 / 3 / 6 month period with no licence fees.

## Prerequisites

* An Azure subscription (required)
* Azure CLI (required)
* A [Partner Center account](lab2-partnercenter.md) with the appropriate permissions (some of the material can be completed without Partner Center access)

## Useful Links

* TBD

## Next

You have the option to choose the  appropriate offer type

* [Lab 5: Publishing an Azure Application Solution Template Offer](lab5-solutiontemplate.md)

## Back

* [Lab 3: Selecting your Offer Type](lab3-offertype.md)
