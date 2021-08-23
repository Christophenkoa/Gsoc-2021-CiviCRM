# Gsoc-2021-CiviCRM
# Multi currency memberships

**Student:** Nkoa Christophe

**Mentors:** Joe Murray, Matthew Wire, Kartik Kathuria 

**Project:** Multi currency Memberships

**Organization:** CiviCRM

**Description:** CiviCRM supports membership payment fees using only dollar currency. Project objective is to create New extension which allows user to pay membership fees through local currency.

## Code
* https://github.com/Christophenkoa/civicrm-core
* https://github.com/Christophenkoa/gsoc_multi_currency_civi_crm

## Repositories involved
* https://github.com/civicrm/civicrm-core
* https://github.com/civicrm/civicrm-buildkit

## Documentation
* https://docs.civicrm.org/

## Install the extension
before the extension been published on civicrm public extension, you can download it [here](https://github.com/Christophenkoa/gsoc_multi_currency_civi_crm) and
install it on your CMS.

## Work done
* Before been able to implement multi currency feature, I notice that multicurrency type table doesn't involve any currency (the table schema doesn't envolve any currency column. It envolves minimum fee without a currency for it). That is why I made a pull on the civi core repository to incorporate it. ([pull link]()).
* I worked also on the UI part. The admin can easily all which currencies the user can use : (image...).
* Also about the UI, I built a good UI to allow a given user to choose a currency for paying its membership fees depending on the one set by the admin (image...). 

 ## TODO
 * Create civicrm_multicurrency_membership_type table which contains a reference to membership_type table.
 * fetch in the public user membership page all membership fees and currencies store in the database because for now it is predifined data which are displayed. 
 * Write unit test.
