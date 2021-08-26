# Gsoc-2021-CiviCRM
# Multi currency memberships

**Student:** Nkoa Christophe

**Mentors:** Joe Murray, Matthew Wire, Kartik Kathuria 

**Project:** Multi currency Memberships

**Organization:** CiviCRM

**Description:** CiviCRM supports membership payment fees using only dollar currency. Project objective is to create New extension which allows user to pay membership fees through local currency.

## Code section

**My extension code** where most of the work has been done.
* https://github.com/Christophenkoa/gsoc_multi_currency_civi_crm

**Commit (civi-core)** where the database schema of the civi core has been altering (membership_type table).
* https://github.com/Christophenkoa/civicrm-core/commit/1999fc709252feb0c0dccaa993106c4cdaff9105

## Repositories involved
* https://github.com/civicrm/civicrm-core
* https://github.com/civicrm/civicrm-buildkit

## Documentation
* https://docs.civicrm.org/
* https://wiki.civicrm.org/

## Install the extension
before the extension been published on civicrm public extension, you can clone it [here](https://github.com/Christophenkoa/gsoc_multi_currency_civi_crm) and
install it on your favorite CMS.

## Work done
* Before been able to implement multi currency feature, I notice that multicurrency type table doesn't involve any currency (the table schema doesn't envolve any currency column. It envolves minimum fee without a currency column for it). That is why I made a pull on the civi core repository to incorporate add a colum currency to membership type table ([pull link]()).

* I worked also on the UI part. The admin can easily add which currencies the user can use : ![screenshot](https://user-images.githubusercontent.com/52603013/130440316-ea185921-3687-4f8e-b7eb-98bb9e489f09.png)
.

* Also about the UI, I built a good UI to allow a given user to choose a currency for paying its membership fees depending on the one set by the admin
![civi_front](https://user-images.githubusercontent.com/52603013/130440184-6986650b-1c7b-456a-8dbc-b9f87e08b2bd.png)
 
 
 ## TODO
 * Create civicrm_multicurrency_membership_type table which contains a reference to membership_type table(currently working on).
 * fetch in the public user membership page all civicrm_multicurrency_membership_type records store in the database because for now it is predifined data which are displayed. 
 * Write unit test.
