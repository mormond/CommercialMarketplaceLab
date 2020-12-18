# Lab 6: Publishing an Azure Application - Managed Application Offer

## Introduction

The *managed application offer* is a type of *Azure App offer*.

*Azure Apps offers* are used to deploy and transact a more complex solution than a single VM. When a customer 'purchases' an *Azure Apps offer*, the solution will be deployed into the customer's Azure subscription. As a consequence, *Azure Apps offers* can only be published in *Azure Marketplace* (not *AppSource*).

*Azure App Offers* support the *Transact* listing type (see below). They also support the *Free* and *BYOL* listing types (and, by offering limited time licences via a *BYOL* listing, support free trials).

The *Azure Apps offer* has two distinct flavours; *solution template* and *managed application*.

* The *solution template* offer is a collection of Azure resources described by an [Azure Resource Manager (ARM) template](https://docs.microsoft.com/azure/azure-resource-manager/templates/overview) which will be deployed into the customer subscription. It is not directly transact-capable but it can deploy *VM Offers* which are transactable.

* The *[managed app](https://docs.microsoft.com/azure/azure-resource-manager/managed-applications/overview)* offer is a collection of Azure resources described by an [ARM template](https://docs.microsoft.com/azure/azure-resource-manager/templates/overview) deployed into the customer subscription to be operated as a managed service (typically managed by the Publisher on behalf of the customer). The customer has limited access to  resources deployed by a managed app. A *Managed App offer* is transactable and can be billed as a flat fee or using *metered billing*.

## Prerequisites

* An Azure subscription (required)
* Azure CLI (required)
* A [Partner Center account](lab2-partnercenter.md) with the appropriate permissions (some of the material can be completed without Partner Center access)

## Useful Links

* TBD

## Next

You have the option to choose the  appropriate offer type

* [Lab 7: Publishing a SaaS Application Offer](lab7-saasapp.md)

## Back

* [Lab 5: Publishing an Azure Application Solution Template Offer](lab5-solutiontemplate.md)
