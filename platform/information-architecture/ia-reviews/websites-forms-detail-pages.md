# IA Review and Recommendations

**Team:** Public Websites

**Product/Featue:** Forms Detail Pages

**Background/Context:**   
These pages will provide a SEO landing page for core form number searches. This is a redesign of existing legacy landing pages. The top forms/online tools will be customized/high-touch while all others will be dynamically generated content via an API.

**Review Date:** _In progress, see open questions/issues at bottom_

**IA Review Issue:** [https://github.com/department-of-veterans-affairs/va.gov-team/issues/3836](https://github.com/department-of-veterans-affairs/va.gov-team/issues/3836)

## IA Structure, URLs and Breadcrumbs 

_Description of IA or link to site map documentation, the final URLs to be used and breadcrumb requirements._

**Structure**

* All form detail pages will be root level pages, they will not be related to or linked to from the forms search tool or elsewhere on the site, except organic search results. 

**URLs**

* All landing pages will have a consistent structured URL that will be dynamically generated from form data. 
  * The form number will be pulled from the forms data and used in the URL preceeded by "/about-form-"  - exact data field TBD
  * Spaces in form numbers will be replaced by dashes
  * All alpha characters will be lower case
  * All characters in the form name/number coming from the data will be used \(i.e. we will not drop extra characters such as "VA"\)

URL Structure: www.va.gov/about-form-\[form-nbr\]

**Drupal URL Requirements**

* Drupal will auto-generate the URL based on the specified form data to complete the URL structure above. 
* The URL, once established, should be locked down so it is not changed if the data is changed
* The auto-generated URL can only be changed by being manually overwritten by the Public Websites team if they choose to do so - changing the URL will likely require redirects to be put in place

**Breadcrumb**

* The breadcrumb will have a consistent structured label that is dynamically generated from form data
  * The form number will be pulled from the forms data and used in the breadcrumb preceeded by "VA form"
  * Spacing and capitalization will be displayed as it is in the data
  * All characters in the form number coming from the data will be used \(i.e. we will not drop extra characters such as "VA"\)

Breadcrumb Structure: Home &gt; VA form \[form number\]

| Example Form data | Example URL | Example Breadcrumb |
| :--- | :--- | :--- |
| 10-10ez | www.va.gov/about-form-10-10ez | Home &gt; VA form 10-10ez |
| 21-526EZ | www.va.gov/about-form-21-526ez | Home &gt; VA form 21-526EZ |
| VA 4107 VHA | www.va.gov/about-form-va-4107-vha | Home &gt; VA form VA 4107 VHA |

## Navigation, Entry Points and Crosslinking 

_The primary entry points and changes to global navigation, as well as any potential crosslinking opportunities_

No navigational links will be added to these pages, users will access these pages directly through external search and va.gov search only.

**User Flows:**

![image.png](https://images.zenhubusercontent.com/59ca6a73b0222d5de4792f1d/ec5630d9-5c71-4ebb-90ab-466cee1d5c8c)

* External search results can/will include a direct link to the online form \(preferred\), a link to the How to Apply page, a link to the form detail page, a direct link to the pdf \(least preferred\).
* VA.gov search results can/will include a direct link to the online form \(preferred\), a link to the How to Apply page, a link to the form detail page, a direct link to the pdf \(least preferred\).
* The Va.gov Find a Form search tool results will only include a direct link to the online form \(preferred\), a link to the How to Apply page, and a direct link to the pdf \(least preferred\).  It _will not_ include a link to these form detail pages.

## Redirects/Canonical 

_Identify if any redirect or canonical tags are needed. This is not intended to be a complete and final list of redirect needs, but directional information only._

* All existing legacy form detail pages will need to be redirected so users do not receive a 404 when trying to visit an old URL from search or old link. 
* We will do server-side redirects of legacy form detail landing pages with the following approach:
  * For X number of high search value form detail landing pages, we will do 1:1 redirect mapping from the current legacy form detail landing page to the new.
  * For the remaining \(562-X\) landing pages, we will do a default redirect to the new main search page URL \(va.gov/find-forms\)
* Specific redirects will be documented in a redirect request ticket.  
* We will need to identify the data source that will be used to generate the URLs for those legacy detail pages that we need to 1:1 redirect.

For redirects, please submit a Redirect Request at least 2 weeks in advance per the [Redirect Request Process](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/information-architecture/request-redirect.md).

## Additional Notes/Recommendations

## Open Questions/Issues

* Facebook currently appends a "fbclid" parameter to URLs when accessed through a link in a FB post.
  * If a specific form page is redirected, will the redirect recognize the request with the additional parameter and redirect appropriately?
  * This can be resolved as part of the redirect process. 
* There are a number of OPM forms that currently have search landing pages and appear in the legacy form search results. Jen will follow up with stakeholders to determine if there is a way to suppress these from showing in the results given they are not VA forms and for internal use only.
  * If they can be suppressed, users will get a "form not found" message
  * If they cannot be suppressed, we will add some of the higher visited forms to our 1:1 redirect list and direct them to either the OPM or GSA site
  * This can be resolved as part of the redirect process. 

