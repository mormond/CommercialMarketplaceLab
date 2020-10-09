# Introduction

Microsoft's commercial marketplace is a catalog of solutions and services from our partner network. Microsoft partners can use Partner Center to create, publish and manage their solutions and services offerings in the commercial marketplace. Solutions are listed in Microsoft's online stores, alongside Microsoft's own solutions, connecting you with businesses, organizations, and government agencies around the world.

This lab will introduce you to some of the essential concepts and terminology of the commercial marketplace with a particular focus on ISVs (Independent Software Vendors) building solutions on Azure. We will focus on cloud solutions rather than services; in other words, how the commercial marketplace caters for cloud solutions built on Microsoft Azure and how to go about publishing them.

## Background Information

* [The Commercial Marketplace documentation](https://docs.microsoft.com/azure/marketplace/overview)
* [What is Partner Center](https://support.microsoft.com/en-us/help/4499930/partner-center-overview)
* [Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace/)
* [AppSource](https://appsource.microsoft.com/)

## Structure

This lab introduces some fundamental concepts and how to choose the best offer type to match a particular solution. The accompanying labs will take you through the steps to create and publish an offer on the commercial marketplace.

* [Lab 1: Introduction to the commercial marketplace](readme.md)
* Lab 2: Publishing a VM Offer
* Lab 3: Publishing an Azure Application Solution Template Offer
* Lab 4: Publishing an Azure Application - Managed Application Offer
* Lab 5: Publishing a SaaS Application Offer

## Terminology

As you might expect, the commercial marketplace has its own vocabulary to describe specific concepts. It's important to understand the specific meanings and how these concepts relate to one another to fully understand commercial marketplace publishing.

* Storefront
  * The *commercial marketplace* has a single backend with [multiple storefronts](https://docs.microsoft.com/en-us/azure/marketplace/overview#commercial-marketplace-online-stores). Published solutions will be listed in one or more *storefronts*.
* Azure Marketplace
  * A *storefront* for solutions aimed at IT professionals.
* AppSource
  * A *storefront* for solutions aimed at business decision makers.
* Offer
  * An *offer* is the vehicle for listing on the *commercial marketplace*. It is a container for all aspects relating to the listing. The listing will appear in one of the *storefronts*.
* Plan
  * *Offers* contain plans which describe the scope (eg in which markets is it available, is it available to everyone or specific customers) and pricing (when applicable).
* Listing Options
  * Transact Offer
    * An offer which is transacted through Microsoft's commerce capabilities and thus delivers an end-to-end experience from discovery to purchase to delivery. Microsoft facilitates the exchange of money for a software licence on behalf of the publisher.
  * List Offer
    * Simple listing of your solution that enables a customer to express interest via *Lead management*.
  * Trial Offer
    * Allow customers to trial your solution for a limited period at no cost before they purchase.
  * BYOL Offer
    * BYOL (Bring Your Own Licence) offers enhance the discoverability and automate the provisioning of your solution in a customer subscription. The financial transaction and licence compliance is the publisher responsibility.
* Test drive
  * A *test drive* is a pre-canned environment that is hosted in the publisher's Azure subscription and allows potential customers to evaluate the solution before purchase.
* Preview audience
  * During the publishing process, an *offer* can be shared with a *preview audience* before it is finally published. Useful for testing purposes.
* Private offers
  * A *private offer* is a plan that is made available to a designated set of customers. This allows for scenarios such as negotiated pricing, private terms & conditions and specialised configurations.
* Lead management
  * *Offers* need to be connected to a lead management system so publishers can be notified about customers interested in deploying their *offers*. This is typically a CRM system but can be a simple Azure table or webhook.
* Categories
  * Each *offer* is listed in a [category or categories](https://docs.microsoft.com/en-us/azure/marketplace/determine-your-listing-type#categories) to aid discoverability. Categories are specific to Azure Marketplace and AppSource.

## Offer Types

The following offer types are available through Partner Center for ISV solutions.

* [Virtual Machine offer](https://docs.microsoft.com/en-us/azure/marketplace/marketplace-virtual-machines)
* [Azure Apps offer - Solution Template](https://docs.microsoft.com/en-us/azure/marketplace/marketplace-solution-templates)
* [Azure Apps offer - Managed Application](https://docs.microsoft.com/en-us/azure/marketplace/marketplace-managed-apps)
* [Container image offer](https://docs.microsoft.com/en-us/azure/marketplace/marketplace-containers)
* [IoT Edge module offer](https://docs.microsoft.com/en-us/azure/marketplace/iot-edge-module)
* [SaaS app offer](https://docs.microsoft.com/en-us/azure/marketplace/plan-saas-offer)

In these labs we will focus on three main offer types; Virtual Machine, Azure Apps and SaaS app offers.

## Virtual Machine Offer

The *Virtual Machine offer* is used to deploy and transact a virtual machine (VM) instance through Marketplace. The solution must consist of only a single VM. Anything more complex requires an *Azure Apps offer*.

When a customer 'purchases' a *VM offer*, the VM will be deployed into the customer's Azure subscription. As a consequence, VM offers can only be published in *Azure Marketplace* (not *AppSource*).

*VM offers* support the *Transact Offer* type. They also support the *BYOL Offer* type (and, by offering limited time licences via a *BYOL Offer*, they also support free trials). A *Test drive* option is also available.

Transact *VM Offers* are billed on a usage-based PAYG (Pay As You Go) model. Each plan can be created with a free trial option giving you the option to offer customers a 1 / 3 / 6 mth period with no licence fees.

## Azure Apps Offer

The *Azure Apps Offer* has two distinct flavours; solution template and managed application.

The solution template is a collection of Azure resources described by an [Azure Resource Manager (ARM) template](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/overview) which will be deployed into the customer subscription. It is not directly transact-capable but it can deploy *VM Offers* which are transactable.

The [managed app](https://docs.microsoft.com/en-us/azure/azure-resource-manager/managed-applications/overview) is a collection of Azure resource described by an ARM template which will be deployed into the customer subscription to be operated as a managed service (typically managed by the Publisher on behalf od the customer). The customer has limited access to the resources deployed by a managed app. A *Managed App offer* is transactable and can be billed as a flat fee or using metered billing.

## SaaS Offer

## Selecting Your Offer Type
