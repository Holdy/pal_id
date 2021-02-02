# Introduction

pal_id (payee and location) is a simple and guessable/repeatable way of allocating ids to business premises. With such ids in place, we can leverage and combine different datasets, and process commercial data from a geographical perspective.

The simplest form of pal_id looks like:

`harrods.com~sw1x_7xl~gb`

It's pretty easy to guess what this is referring to, as we've simply taken three components and joined them with a tilde:

(`basic webdomain`) ~ (`store postcode`) ~ (`2 letter country for good measure`)

So far, so good, but Harrods is a pretty unique place (in the UK at least), it's more useful to differentiate chain stores - here are 3 of the many Tesco stores in Norwich, Norfolk:

`tesco.com~nr6_6xa~gb`<br/>
`tesco.com~nr2_2rw~gb`<br/>
`tesco.com~nr1_3lg~gb`

Tesco and the other supermarket chains often have on-site petrol stations which will almost always share a postcode with the associated store - so we differentiate them with a prefix:

`tesco.com~nr7_8ab~gb` - A store just like the 3 above.<br/>
`(petrol)tesco.com~nr7_8ab~gb` - The on site petrol station.

<em>NOTE: 'petrol' seems like we're forgetting diesel and LPG, but they're all petrol(ium) at heart.</em>

These prefixes like (petrol) are used when a company has deviated from its core business. other prefixes we will see are:

 `(pharmacy)` - differentiates from 'normal' co-op stores.
 
 `(mobile)` - differentiates (for example) skys phone/sim/tablet business from the TV channel

 `(parking)` - For stores with a pay-and-display carpark, or government carparks.

 `(recycling)` - Again those pesky governments providing multiple facilities.

 `(atm)` - Always used on cash machines

 So far we've covered physical stores, but we can also do web:

`tesco.com~online~gb` we may know its a bricks-and-mortar store, but we don't know where `tesco.com~_~gb` and if we're not sure `tesco.com~~gb`
