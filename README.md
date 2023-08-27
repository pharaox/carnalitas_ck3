# Carnalitas EK2 Compatibility

This is a [Carnalitas](https://www.loverslab.com/files/file/14207-carnalitas-unified-sex-mod-framework-for-ck3/) compatibility patch for CK3 1.10. It reconciles changes to the character window, the court window and other files that were changed incompatibly in CK3 compared to the latest released versions of Carnalitas.

The latest version is based on Carnalitas 2.0 (for CK3 1.9) and compatible with CK3 1.10.0.

Load order:

* Carnalitas
* Carnalitas Patch for CK3 1.10
* (other mods based on Carnalitas)

## Compatibility Fixes

### Character and Court Windows

All changes to the character and court windows made by Carnalitas and CK3 1.10 have been reconciled, so that all additional interface elements introduced by both are present. This means that *Home Court* and *Warden* icons for wards and filtering by *Hostages* that were introduced by CK3 1.10, as well as Carnalitas *Slaves* at the bottom of the *Relationships* tab, are all properly shown.

### Interactions, Schemes, Triggers, and Events

All changes to interactions, schemes, triggers, and events made by Carnalitas and CK3 1.10 have been reconciled. The CK3 files have been taken as base, and Carnalitas changes have been applied on them. For 2 of the files, their versions from [Unofficial Patch](https://steamcommunity.com/sharedfiles/filedetails/?id=2871648329) for CK3 1.10 have been taken as base, since they contain a few important fixes that would otherwise be lost, since that mod should be first in the load order if used.

The main effects (compared to the unpatched Carnalitas 2.0) are the following:

* The *Grant Titles* interaction properly checks new conditions introduced in CK3 1.10, such as whether the recipient is a hostage (`grant_titles_interaction`)
* It is not possible to abduct a hostage (`abduct` scheme)
* A character can't contract an STD while traveling if they are involved in a *University Visit* activity (`can_contract_disease_trigger`)
* Fixes to some birth and pregnancy events for issues in CK3 1.9 (and a few more fixes from the Unofficial Patch)
