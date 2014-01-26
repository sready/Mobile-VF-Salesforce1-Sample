# VF Example - Salesforce1 Webinar 1/22/14

This sample package contains the page and controller necessary to create create a volunteer record on submit and relate a picture to it. In the sample, the flow is as follows: 
1. The volunteer record is created
2. The photo file that was grabbed in JavaScript is then used to create a chatter file
3. The ID of the image is then stored to a hidden field on the volunteer record and the record is updated

This field can be used to create a formula field of the image on the record, or as a reference for the picture elsewhere like in a VF page inlaid as a mobile card. There is more detail on this kind of functionality explicitly in [Pat's blog](http://blogs.developerforce.com/developer-relations/2013/12/salesforce1-cures-the-app-boogie-fever.html). 

You can install the simple schema to your DE with this unmanaged package:
https://login.salesforce.com/packaging/installPackage.apexp?p0=04ti00000004NmK

To test out the page, create one volunteer event with a geolocation coordinate within 3 miles of your current location. I did not include remote site settings or any geocoding Apex classes in this package. Once you have a volunteer event nearby, create a tab for the page, and add it to mobile navigation. 
