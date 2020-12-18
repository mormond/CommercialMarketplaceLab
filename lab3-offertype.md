# Lab 3: Selecting your Offer Type

## Introduction

Now we are familiar with some of the key terminology and characteristics of the different offer types, it's time to determine which offer type is best suited for your solution.

## Selecting Your Offer Type

The previous section will have given you a good feel for the characteristics of the different offer types

In these labs we are focussing on the main offer types that have provisioning and transact capability; *VM Offer*, *Azure App Offer* and *SaaS App Offer*.

Your first decision point will likely be how the solution is deployed.

* If it's a SaaS application that runs in the publisher's Azure subscription then it will be a *SaaS App Offer*.
* If the solution gets deployed into the customer subscription then it will be either a *VM Offer* or an *Azure App Offer*. If it's a single virtual machine it will be a *VM Offer*.
* If it's more than a single virtual machine then it comes down to who will manage the solution.
  * If the customer will be responsible the best match is an *Azure App Offer - Solution Template*.
  * If the customer wants it to be managed on their behalf it will be an *Azure App Offer - Managed Application*.

Note the limitations in Lab 1 with respect to *Azure App Offers*. Solution templates are not directly transactable but can be made so by referencing *VM Offers*. Managed applications grant the customer limited access and require the solution to be managed on their behalf.

## Next

You have the option to choose the  appropriate offer type

* [Lab 4: Publishing a VM Offer](lab4-vmoffer
* .md)
* [Lab 5: Publishing an Azure Application Solution Template Offer](lab5-solutiontemplate.md)
* [Lab 6: Publishing an Azure Application - Managed Application Offer](lab6-managedapp
* .md)
* [Lab 7: Publishing a SaaS Application Offer](lab7-saasapp.md)

## Back

* [Lab 2: Enroll in Partner Center to Publish Offers](lab2-partnercenter.md)
