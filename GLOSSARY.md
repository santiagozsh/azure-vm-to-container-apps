# Real Estate Listings Platform

A simulated real estate agency system, inherited from a freelancer as a single hand-built VM, and migrated to managed Azure services.

## Real estate domain

**Property**:
The physical real estate asset (house, apartment, lot) that exists in the world.
_Avoid_: Unit, asset, building

**Listing**:
The published article on the web app that advertises a Property for sale or rent.
_Avoid_: Product, post, ad, property (when meaning the published article)

**Photo**:
An image attached to a Listing.
_Avoid_: Picture, image, media

**Catalog**:
The public-facing landing where visitors browse published Listings.
_Avoid_: Storefront, landing, home

**Admin Panel**:
The private area where agency staff create, edit, and remove Listings and their Photos.
_Avoid_: Dashboard, backoffice, CMS

## Migration story

**Legacy System**:
The inherited deployment: web, API, database, and Photos all running on a single hand-provisioned VM.
_Avoid_: Old system, monolith, VM version

**Cutover**:
The moment traffic and data move from the Legacy System to the new platform, after which the Legacy System is destroyed.
_Avoid_: Switchover, go-live
