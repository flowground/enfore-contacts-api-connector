# ![LOGO](logo.png) enfore Contacts API **flow**ground Connector

## Description

A generated **flow**ground connector for the enfore Contacts API API (version 0.3.1).

Generated from: http://localhost<br/>
Generated at: 2019-11-14T14:44:41+02:00

## API Description

enfore API for managing contacts (incl. customers and suppliers)<br/>
<br/>
Contacts are entities that the organization has dealings with.<br/>
Contacts can be split into individual contacts (i.e., human persons) and organization contacts (i.e., other organizations/businesses).<br/>
Additionally, contacts can have roles such as being a supplier or a customer. A single contact can have multiple roles. I.e., a supplier can also be a customer.<br/>

## Authorization

This API does not require authorization.

## Actions

### Load all individual contacts from an organization

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `limit` - _optional_ - Max number of objects to be returned per page.<br/>
Note that both the `items` as well as the `problems` arrays of the query response count towards this number to allow a simple,<br/>
consistent paging over all items (and problems) of a given timeframe.<br/>
If not given, defaults to `200`.<br/>
* `offset` - _optional_ - Offset of items and problems of where to start the next page.<br/>
Similar to limit and offset in SQL, one would obtain the second page with `limit=10&offset=10`.<br/>
Note that this paging with limit and offset is within a time interval that is specified with `from` and `to`.<br/>
If not given, defaults to `0`.<br/>

### Add a new IndividualContact to the organization

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>

### Load an IndividualContact by its identifier

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Full update of an IndividualContact

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Load an IndividualContact with Subresources by its identifier

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Get all addresses of a contact.

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Add a new address to a contact

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Load an address by parent contact and identifier

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `address-id` - _required_ - ID of the address<br/>

### Full update of an address

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `address-id` - _required_ - ID of the address<br/>

### Get all emails of a contact.

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Add a new email to a contact

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Load an email by parent contact and identifier

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `email-id` - _required_ - ID of the email<br/>

### Full update of an email

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `email-id` - _required_ - ID of the email<br/>

### Get all phones of a contact.

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Add a new phone to a contact

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Load an phone by parent contact and identifier

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `phone-id` - _required_ - ID of the phone<br/>

### Full update of an phone

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `phone-id` - _required_ - ID of the phone<br/>

### Get all web addresses of a contact.

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Add a new web address to a contact

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Load a web address by parent contact and identifier

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `web-address-id` - _required_ - ID of the address<br/>

### Full update of a web address

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `web-address-id` - _required_ - ID of the address<br/>

### Get the mapping of internal to external IDs for individual contacts.

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `external-id` - _required_ - External ID for which an internal ID should be returned.<br/>

### Get the mapping of internal to external IDs for individual contacts.

*Tags:* `Individual Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>

### Get all professional identities of an IndividualContact.

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Add a new professional identity to an IndividualContact

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Get all professional identities with Subresources of an IndividualContact.

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Load a ProfessionalIdentity by parent contact and identifier

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the ProfessionalIdentity<br/>

### Full update of a ProfessionalIdentity

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the ProfessionalIdentity<br/>

### Load a ProfessionalIdentity with Subresources by parent contact and identifier

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the ProfessionalIdentity<br/>

### Get all addresses of a professional identity of a contact.

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity<br/>

### Add a new address to a professional identity of a contact

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity<br/>

### Load an address by parent contact, professional identity and identifier

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity the address belongs to<br/>
* `address-id` - _required_ - ID of the address<br/>

### Full update of an address

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity the address belongs to<br/>
* `address-id` - _required_ - ID of the address<br/>

### Get all emails of a professional identity of a contact.

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity the emails belong to<br/>

### Add a new email to a professional identity of a contact

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity the emails belong to<br/>

### Load an email by parent contact, professional identity and identifier

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity the email belongs to<br/>
* `email-id` - _required_ - ID of the email<br/>

### Full update of an email

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity the email belongs to<br/>
* `email-id` - _required_ - ID of the email<br/>

### Get all phones of a professional identity of a contact.

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity the phones belong to<br/>

### Add a new phone to a professional identity of a contact

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity the phones belong to<br/>

### Load an phone by parent contact, professional identity and identifier

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity the phone belongs to<br/>
* `phone-id` - _required_ - ID of the phone<br/>

### Full update of an phone

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity the phone belongs to<br/>
* `phone-id` - _required_ - ID of the phone<br/>

### Get all web addresses of a professional identity of a contact.

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity the addresses belong to<br/>

### Add a new web address to a professional identity of a contact

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity the addresses belong to<br/>

### Load a web address by parent contact, professional identity and identifier

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity the address belongs to<br/>
* `web-address-id` - _required_ - ID of the address<br/>

### Full update of a web address

*Tags:* `Individual Contacts: Professional Identities`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `professional-identity-id` - _required_ - ID of the professional identity the address belongs to<br/>
* `web-address-id` - _required_ - ID of the address<br/>

### get_org__org_id__individual__contact_id__roles_customer

*Tags:* `Individual Contacts: Roles`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### put_org__org_id__individual__contact_id__roles_customer

*Tags:* `Individual Contacts: Roles`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### get_org__org_id__individual__contact_id__roles_supplier

*Tags:* `Individual Contacts: Roles`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### put_org__org_id__individual__contact_id__roles_supplier

*Tags:* `Individual Contacts: Roles`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Load all organization contacts from an organization

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `limit` - _optional_ - Max number of objects to be returned per page.<br/>
Note that both the `items` as well as the `problems` arrays of the query response count towards this number to allow a simple,<br/>
consistent paging over all items (and problems) of a given timeframe.<br/>
If not given, defaults to `200`.<br/>
* `offset` - _optional_ - Offset of items and problems of where to start the next page.<br/>
Similar to limit and offset in SQL, one would obtain the second page with `limit=10&offset=10`.<br/>
Note that this paging with limit and offset is within a time interval that is specified with `from` and `to`.<br/>
If not given, defaults to `0`.<br/>

### Add a new OrganizationContact to the organization

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>

### Load an OrganizationContact by its identifier

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Full update of an OrganizationContact

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Load an OrganizationContact with Subresources by its identifier

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Get all addresses of a contact.

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Add a new address to a contact

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Load an address by parent contact and identifier

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `address-id` - _required_ - ID of the address to load<br/>

### Full update of an address

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `address-id` - _required_ - ID of the address to load<br/>

### Get all emails of a contact.

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Add a new email to a contact

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Load an email by parent contact and identifier

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `email-id` - _required_ - ID of the email to load<br/>

### Full update of an email

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `email-id` - _required_ - ID of the email to load<br/>

### Get all phones of a contact.

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Add a new phone to a contact

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Load an phone by parent contact and identifier

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `phone-id` - _required_ - ID of the phone<br/>

### Full update of an phone

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `phone-id` - _required_ - ID of the phone<br/>

### Get all web addresses of a contact.

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Add a new web address to a contact

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### Load a web address by parent contact and identifier

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `web-address-id` - _required_ - ID of the web address<br/>

### Full update of a web address

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>
* `web-address-id` - _required_ - ID of the web address<br/>

### Get the mapping of internal to external IDs for organization contacts.

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `external-id` - _required_ - External ID for which an internal ID should be returned.<br/>

### Get the mapping of internal to external IDs for organization contacts.

*Tags:* `Organization Contacts`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>

### get_org__org_id__organization__contact_id__roles_customer

*Tags:* `Organization Contacts: Roles`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### put_org__org_id__organization__contact_id__roles_customer

*Tags:* `Organization Contacts: Roles`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### get_org__org_id__organization__contact_id__roles_supplier

*Tags:* `Organization Contacts: Roles`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

### put_org__org_id__organization__contact_id__roles_supplier

*Tags:* `Organization Contacts: Roles`

#### Input Parameters
* `org-id` - _required_ - ID of the organization whose data is being accessed.<br/>
* `contact-id` - _required_ - ID of the contact<br/>

## License

**flow**ground :- Telekom iPaaS / enfore-contacts-api-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
