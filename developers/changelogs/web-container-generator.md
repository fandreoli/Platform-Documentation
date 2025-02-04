# Web container generator

## 2023

### Release v81.0 - 14/02/2023

* Internal upgrade of the generator server. Greatly improves generator performance. This upgrade should not impact the generation result, though we recommend that you test your first generated container before your next deployment.

### Release v80.3 - 08/02/2023

* Refactoring on various TagCommander modules

### Release v80.2 - 08/02/2023

* Add tc_privacy_do_not_track flag
* Refactoring on the TagDeduplication

### Release v80.1 - 24/01/2023

* Refactoring on the tC.privacy module

### Release v80.0 - 17/01/2023

* Add new Consent OnSite API commands:
  * `consent.onReady`
  * `consentBanner.show`
  * `consentBanner.hide`
  * `consentCenter.show`
  * `consentCenter.hide`

### Release v79.1 - 16/01/2023

* Refactoring on the Privacy Banners

### Release v79.0 - 12/01/2023

* Refactoring on the tC object initialization

## 2022

### Release v78.0 - 13/12/2022

* Update `tC.setCookie` to encode `!'()~` characters in the cookie value. This is a requirement for WAF restrictions of some TagCommander users.

### Release v77.0 - 01/12/2022

* Update `tC.privacy.hit` to not send hits when analytics category was refused using consent JS OnSite API

### Release v76.1 - 30/11/2022

* Update `trigger` JS OnSite API to better use source-keys in multi-container contexts

### Release v76.0 - 15/11/2022

* Update `tC.setCookie` to use `encodeURIComponent` instead of `escape` (deprecated)

### Release v75.3 - 19/09/2022

* Update page data format in `cact('trigger')` API

### Release v75.2 - 15/09/2022

* Refactoring on privacy hits generation

### Release v75.1 - 02/08/2022

* Better handling of old .tagcommander.com domain redirections on Tag Deduplication

### Release v75.0 - 19/07/2022

* Improve tC.privacy.getCategoryIdList

### Release v74.1 - 13/07/2022

* Fix domain detection

### Release v74.0 - 06/07/2022

* Do not mutate `cact()` arguments

### Release v73.0 - 05/07/2022

* Automatically integrate domains set up in Domain Management

### Release v72.1 - 20/06/2022

* Make consent data available in `consent.get` before privacy file is loaded

### Release v72.0 - 18/05/2022

* Add refused_vendors in CAX events

### Release v71.1 - 26/04/2022

* Fix blocked on categories not sent in CAX events

### Release v71.0 - 18/01/2022

* Integrate TrustCommander settings with DataStorage cookies

### Release v70.0 - 13/04/2022

* Commanders Act - Platform X Source keys enabled on all web containers

### Release v69.1 - 05/04/2022

* Add page and device information in OneTag events

### Release v69.0 - 22/03/2022

* Improve TrustCommander event format. `list_categories` is renamed `optin_categories`. `optout_categories` are now included in the event.

### Release v68.1 - 24/01/2022

* Improve setCookie domain detection

### Release v68.0 - 18/01/2022

* Tag Deduplication - Add a (programatic) option to not use tc_cj_v2 encryption. This is a requirement for WAF restrictions of some TagCommander users.

## 2021

### Release v67.1 - 07/12/2021

* Store generated versions on remote server (no more NFS usage)

### Release v67.0 - 03/12/2021

* Fix tC.log escaping

### Release v66.0 - 02/12/2021

* Fix minor tags generation

### Release v65.0 - 24/11/2021

* Integrate `tC.trigger` / `cact('trigger')` natively  inside web containers

### Release v64.0 - 18/10/2021

* Tag Deduplication - Fix campaign/medium cookie initialization

### Release v63.0 - 07/10/2021

* Include blocked on categories in Privacy hits

### Release v62.0 - 07/09/2021

* Refactoring on Privacy Banner Templates

### Release v61.0 - 28/06/2021

* Tag Deduplication - Fix launcher on "bypass" setups

### Release v60.0 - 31/05/2021

* TrustCommander - Fix analytics for setups where it is set as blocked on category

### Release v59.0 - 15/04/2021

* TrustCommander - Fix `tC.privacy.getBlockedOnCategories`

### Release v58.0 - 25/02/2021

* Add new Consent OnSite APIs:
  * `consent.onUpdate`
  * `consent.update`
  * `consent.revoke`

### Release v57.0 - 23/02/2021

* Add `consent.get` OnSite API

### Release v56.0 - 09/02/2021

* Privacy - Rework parameters inclusion

### Release v55.0 - 26/01/2021

* Privacy - Fix categories statistics sending

### Release v54.0 - 11/01/2021

* Privacy - Fix missing TCID on some opin hits

## 2020

### Release v53.0 - 12/11/2020

* Privacy - Optimize vendor statistics when visitor is optin to all vendors

### Release v52.0 - 19/10/2020

* TrustCommander - Integrate Google ACM

### Release v51.0 - 16/10/2020

* Improve generator performance

### Release v50.0 - 15/10/2020

* Update vendor statistics format

### Release v49.0 - 17/09/2020

* Fix optional modules inclusion in unminified web containers

### Release v48.0 - 20/08/2020

* Fix TC_PRIVACY cookie content caused by a retro-compatibility issue with old banners

### Release v47.0 - 18/08/2020

* Fix privacy vendors initialization

### Release v46.0 - 17/08/2020

* Fix privacy vendors usage in TMS

### Release v45.0 - 14/08/2020

* Integrate __tcfapi stub

### Release v44.0 - 06/07/2020

* Use privacy vendors in TMS

### Release v43.0 - 28/05/2020

* Set consent duration by Privacy banner

### Release v42.0 - 29/04/2020

* Fix vendor encoding in web containers

### Release v41.0 - 20/04/2020

* Fix tC.events sorting

### Release v40.0 - 24/02/2020

* Fix internal variable initialization on container reload

### Release v39.0 - 24/02/2020

* Fix internal variable initialization on container reload

### Release v38.0 - 11/02/2020

* Deactivate tC reach

### Release v37.0 - 03/02/2020

* Fix privacy statistics on optin all

### Release v36.0 - 21/01/2020

* Fix privacy statistics intialization from container

### Release v35.0 - 20/01/2020

* Fix privacy statistics intialization from container

### Release v34.0 - 09/01/2020

* Fix Tag Deduplication initialization on container reload

## 2019

### Release v33.0 - 07/11/2019

* Do not run Privacy code when cookies are disabled

### Release v32.0 - 07/11/2019

* Refactoring on generator code base

### Release v31.0 - 07/11/2019

* Fix tC.event initialization on container reload

### Release v30.0 - 06/11/2019

* Fix to avoid reloading tC.event when triggred on Dom Ready

### Release v29.0 - 01/10/2019

* Fix conflict between containers when initializating internal variables

### Release v28.0 - 25/09/2019

* Fix Tag Deduplication by merging config when multiple containers are on the same page

### Release v27.0 - 18/09/2019

* Add `tC.isCookieEnabled`

### Release v26.0 - 25/07/2019

* Add more details for privacy statistics on optin all

### Release v25.0 - 10/06/2019

* Security fix

### Release v24.0 - 30/05/2019

* Fix platform user rights

### Release v23.0 - 28/05/2019

* Fix privacy analytics

### Release v22.0 - 28/05/2019

* Fix TCPID in privacy analytics

### Release v21.0 - 28/05/2019

* Add option to disable TCPID

### Release v20.0 - 29/04/2019

* Privacy - add custom separator and domain

### Release v19.0 - 08/04/2019

* Fix custom events to work without second argument

### Release v18.0 - 05/04/2019

* Fix tc_array_events object initialization

### Release v17.0 - 20/03/2019

* Refactoring for Privacy Standalone

### Release v16.0 - 02/03/2019

* Fix privacy analytics

### Release v15.0 - 21/02/2019

* Fix `tC.array_launched_tags` initialization

### Release v14.0 - 16/01/2019

* Fix `tC.privacy.validRules` initialization

### Release v13.0 - 14/01/2019

* Refactoring on Privacy Templates (Privacy v2)

### Release v12.0 - 07/01/2019

* Add custom privacy default status (optin/optout) for tags

## 2018

### Release v11.0 - 15/08/2018

* Add option to set default privacy default status (optin/optout) for banners

### Release v10.0 - 10/08/2018

* Privacy - On Premise option

### Release v9.0 - 08/10/2018

* Fix Browser Extension error

### Release v8.0 - 01/10/2018

* Fix tC.event on mutli-container contexts

### Release v7.0 - 17/09/2018

* Fix Dom Ready Trigger

### Release v6.0 - 12/06/2018

* Handle dynamic change of version from Browser Extension

### Release v5.0 - 11/04/2018

* Initial release of TagCommander v2
