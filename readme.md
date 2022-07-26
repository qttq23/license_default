
# 1. open source

## codebase:

### LICENSE: 
is contract between author and user.
a license lists out what users can and cannot do with a product.
a license also states what author provides and not provides.

if a product/project has no license, no one can legally use it because they have no idea about how to use it.
when you provide a license to your product/project, you have provided a way for your users to use your products.

3 common types of license:
permissive: (MIT, BSD, Apache 2.0)
users can use the product or modify and then distribute it under any other license. 
the only condition is that the copyright and the permissive license must be kept along with other licenses.
-> recommended.

lesser copyleft: (LGPL 2.1 or 3.0, Mozilla Public License, Eclipse Public License)
if you use lesser copyleft component separately (dynamic link), you can license your whole product with any license you want.
-> in practise, this is enough.

if you use lesser copyleft component internally (static link), you have to show how you integrate it to your app such as how to build your app with the copyleft component.
if you modify the lesser copyleft component, you have to point out what you have modified.

(
https://fossa.com/blog/open-source-software-licenses-101-lgpl-license/
)

copyleft: (GPL v2, v3)
if any copyleft component exists in your product, the whole product and every component in side it must be copyleft licensed too.
this means you have to public everything including your code and the libraries you depend on.
-> not recommended, because it restricts your app from propietary later.

(
references:
https://fossa.com/blog/what-do-open-source-licenses-even-mean/
https://fossa.com/blog/apply-license-open-source-software-project/
)


### NOTICE
NOTICE file is to write which part of your project is not licensed the same as the LICENSE file or different copyright owner.

https://opensource.stackexchange.com/questions/7872/how-to-properly-assemble-notice-file-for-new-software-under-apache-license-2-0


### CONTRIBUTORS 
if you join a company, you may have to sign the document similar to CLA (contributor licensing agreement).
if you contribute a open source, you may have to agree on CLA for your pull request to be approved. (not all open source projects requires this)

this CLA generally states that your copyright is remains to you but the company or the project's owner has the right to change project's license at later version.
the project with multiple contributors usually has the CONTRIBUTORS file to list out the contributors.

later time, if the project's owner wants to change license, he can just change it without your consent because you already agreed on the CLA.

if the project didn't require CLA, then the project's owner has to ask every contributors' permissions to able to change the license. 
it makes sense because the time you join project and contribute, you hope that your work will remain public and help others. 
it will be ridiculous if the owner just change the license to proprietary and dont ask your permission.

(
the section 'Copyright and Contributor Licensing Agreement' at:
https://fossa.com/blog/apply-license-open-source-software-project/
)

### copyright notice

copyright notice in file:
make it clear that the file is belongs to someone.
invite the users to use this file in the case of permissive license.
give users notice not to use this file in the case of more restricted license.
-> not mandatary, but recommended in practice.

(
https://qr.ae/pvklZK
)

multiple contribution to a file:
put multiple notice in the header of file or header of a function.
do not delete the old notice.

https://opensource.stackexchange.com/questions/886/copyright-and-contributing-to-an-open-source-project/?fbclid=IwAR1f-OFLiWWrWQEzYsEx_mIkk_EFnx58p-QBz0jjwHqP69IeHXP9V6OEsMM


copyright notice in web:
not require but should put at least in the footer of homepage.

eg: 
copyright 2019 johny adam, all rights reserved.
(this means you donot share the right to use your content to anyone)

or:
copyright 2019 johny adam, no rights reserved.
(this means everyone can use content of your page.)

https://www.legalzoom.com/articles/when-and-where-to-use-a-copyright-notice?fbclid=IwAR0gp3-l7GBJxX8-RHNLT1WFtcSIxVTZJhECzpUXn_2BNkHbeNdx05IxCv0


## binary base:

### cookie policy:

cookies is what you store in client's machine. (include https's cookies, html5's localStorage, sessionStorage,..)
if you store only data for your app to work smoothly and you don't need those for processing in backend and don't transfer data to 3rd, you don't need to ask for user consent.
examples:
- store login info for later quick login
- store accessed links for highlighting.
- store preferences about colors, settings.

if you store data in client then pull it for processing such as analysing user's behaviors, or if you transfer or sell user data to 3rd party, you must have cookie policies and get user consent.
examples:
- store user's info for counting how many active users at the present.
- analysing user's orientation/trending.
- sell/transfer user's cookies to 3rd.

cookie consent usually appears at the firstime user visits a website. cookies consent should a link to cookie policy.

details:
https://termly.io/resources/articles/types-of-internet-cookies/

https://softwareengineering.stackexchange.com/questions/290566/is-localstorage-under-the-cookie-law

to generate:
https://www.cookiepolicygenerator.com/cookie-policy-generator/


### privacy policy:

tell users what you do with the data about users in backend such as email, password, address, description,...
and tell users what do with the data about users in frontend (cookie policy if you use it)

examples:
- what info you get from users?
- what purposes of those info ?
- how you secure user info ?
- do you give user info to 3rd ?
- can user change info or withdraw such as delete account, if so how you deal with those cases ?

privacy policy usually appears in the process of creating new account. users have to check box to accept and create an account.

details:
https://www.freeprivacypolicy.com/blog/write-privacy-policy/#What_Is_A_Privacy_Policy


to generate:
go to:
https://app.termly.io/dashboard

click: Policies > Privacy Policy
remember to delete the old privacy to publish new one.


### cookie policy vs privacy policy:
cookie policy only applies to what is stored in client's machine.
privacy policy applies both to what is stored in client's machines and backend.
so if you store info in backend, you must have privacy policy and in that privacy policy, include a link to cookie policy (if cookie policy is required).

https://www.cookiebot.com/en/cookie-policy/


### EULA
same as License. 
retain the copyright.
grant end-user permission to use the software.
state what users can and cannot do regarding the use of software.

EULA usually presents in the installation process of desktop app or in the opening screen of mobile app after installing. uses have to accept to continue.
(user have a copy of application)

details:
https://termly.io/resources/articles/what-is-eula/

to generate:
go to:
https://app.termly.io/dashboard

click: Policies > EULA
remember to delete the old privacy to publish new one.

(or go to: https://easylegaldocs.com/templates/agreements/eula/)


### terms of services
(as known as terms and conditions or terms of use)

define what end-users can and cannot do regarding actions inside the service 
such as community guidelines, good/bad behaviors, conditions to ban/disable user account.
also define copyright and use of software.

terms of services usually presents in the bottom of website. and officially confirmed when user creates an account.
(user doesnot have a copy of application, they just use browser to access website)

details:
https://www.iubenda.com/en/help/2859-terms-and-conditions-when-are-they-needed

to generate:
go to:
https://app.termly.io/dashboard

click: Policies > Terms and Conditions
remember to delete the old privacy to publish new one.

### EULA vs terms of services
eula is about copyright and use of software. it is like a license.
terms of services is about both license and what proper behavior of uses inside app/services. terms of services can include a link to EULA.

if you deliver an local app (desktop or mobile), you should a an EULA document for user to accept. because they have a copy of your product.
then you can opt in a Terms of Services document if you define user behaviors in app.

if you deliver a service (website), you don't need EULA, but you will need Terms of Services which defines proper user behaviors in service.


http://www.differencebetween.info/difference-between-eula-and-terms-of-use



### others

community standards/guildlines ??


needs to put LICENSE in binary: no
copyright notice in software, website: presents in EULA or Terms of Services.


# Proprietary software: ??

