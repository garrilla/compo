## Principles

This document is an evolving set of princples for the design of **Quartz** compenents for **Meteor JS**

  - *no __principle__ can be abrogated within a branch*
  - *no __principle__ should conflict any other princple* 

###Open

**Quartz** and any branch projects should be open source.

###Licensed

A licence should be set that allows forking, developement but maintains attribution to the original source, maintaining a **_principled_** approach.

###Re-usable

All compenents are to be re-useable.
> in this context "re-use" should mean that no component is restricted in it use by virtue of having defined `id`, components should be able to be used more than one on a page, should be invoked by reference to a *quartz* template blocke `{{> quartz}}` with its purpose and context set by an extensible set parameters to the template block as data attributes `{{> quartz type="menu" subtype="nav" id="someId" content="foo" source="collection"}}`

###Re-active

All components should be reactive, using the defaultt **Meteor JS** code syntax and styling. 

###Framework Agnostic

**Quartz** components should be framework agnostic, but where practicable, should be styleable through the *quartz* template block

###Packagable

Each component should be created as package within the **Meteor JS** so there is a standard reference, e.g. `quartz:menu`, `quartz:carousel`, `quartz:message` etc

###Unlimited depdendecies

Compenent packages can be dependent on other packages or **Npm modules** 
> this is potentially an area where the *princple of no conflict* could be of importance, for example a component could not be depndent on package that is style for bootstrap-3

###Declared dependecies

Compenent packages should declare all depndencies, no assumptions should be made about **Meteor JS** packages as these are being slowly deprecated. 

