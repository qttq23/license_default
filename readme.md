
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


binary base: ??
 needs to put LICENSE ??
 EULA ?
 Terms of service ?
 Privacy Policies ?
 community standards ?
 copyright notice in software, website??


# Proprietary software: ??

