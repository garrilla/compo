## Principles

This document is an evolving set of princples for the design of **Quartz** compenents for **Meteor JS**

###Open

The project should be open source.

###Licensed

A licence should be set that allows forking, developement but maintains attribution to the original source.

###Re-usable

All compenents are to be re-useable.
> in this context "re-use" should mean that no component is restricted in it use by virtue of having defined `id`, components should be able to be used more than one on a page, should be invoked by reference to a *quartz* template blocke `{{> quartz}}` with its purpose and context set by an extensible set parameters to the template block as data attributes `{{> quarzt id="myFooMenu" type="menu" content="foo"}}`

###Re-active

All components should be reactive, using the defaultt **Meteor JS** code syntax and styling. 

###Framework Agnostic

**Quartz** components should be framework agnostic, but where practicable, should be styleable through the 

###Packagable

Each component should be created as package within the **Meteor JS** so there is a standard reference, e.g. `quartz:menu`, `quartz:carousel`, `quartz:message` etc

###Unlimited depdendecies

Compenents can be depndednt on other packages or **Npm modules**

