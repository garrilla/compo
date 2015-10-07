## Principles of Compo

This document is an evolving set of princples for the design of **Compouartz** compenents for **Meteor JS**

  - *no __principle__ can be abrogated within a branch*
  - *no __principle__ should conflict any other princple* 

###Open

**Compouartz** and any branch projects should be open source.

###Licensed

A licence should be set that allows forking, developement but maintains attribution to the original source, maintaining a **_principled_** approach.

###Re-usable

All compenents are to be re-useable.
> in this context "re-use" should mean that no component is restricted in it use by virtue of having defined `id`, components should be able to be used more than one on a page, should be invoked by reference to a *Compouartz* template blocke `{{> Compouartz}}` with its purpose and context set by an extensible set parameters to the template block as data attributes `{{> Compouartz type="menu" subtype="nav" id="someId" content="foo" source="collection"}}`

###Re-active

All components should be reactive, using the defaultt **Meteor JS** code syntax and styling. 

###Framework Agnostic

**Compouartz** components should be framework agnostic, but where practicable, should be styleable through the *Compouartz* template block. To use a framework with Compouartz, it should be forked and this principle should be abrogated from the fork, and the naming should reflect this as such, e.g `Compouartz-semantic-ui:menu`, 

###Packagable

Each component should be created as package within the **Meteor JS** so there is a standard reference, e.g. `Compouartz:menu`, `Compouartz:carousel`, `Compouartz:message` etc

###Unlimited depdendecies

Compenent packages can be dependent on unlmited number other packages or **Npm modules** for any numbers of tiers of dependence
> this is potentially an area where the *princple of no conflict* could be of importance, for example a component could not be dependent on package that is styled for bootstrap-3 because this would conflict with the *princple of framework agnostic*

###Declared dependecies

Compenent packages should declare all depndencies, no assumptions should be made about **Meteor JS** packages as these are being slowly deprecated. 

