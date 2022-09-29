###Tech Stack
Frontend Language : HTML, CSS, JavaScript

Backend Language : PHP

Server : Apache

Programming Style : Object Oriented Programming Style for Backend

Mailing Service : PHP mail() function with help of sendmail integrated with Amazon

####--Email a random XKCD challenge--##
This PHP application accepts a visitor’s email address and then verifies the email address with OTP(One Time Password) sent to the visitor's email and after verification random XKCD comics will be sent in every five minutes including the inline image content as well as attachment. User can also Unsubscribe from the email service at any time. Application also contains the Admin Panel to manage all the users in Graphical Interface

Subscription
Un-subscribe
Admin Panel
#####-----Random XKCD comics------#####

Every verified/subscribed user will get random XKCD comics on his/her email id in every 5 minutes, email will contain an attachment along with the inline image as well as comic content. To fetch the comic data, https://c.xkcd.com/random/comic is used programmatically to return a random comic URL which then further sanitize and then use to get all data for content.

