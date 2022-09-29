###Tech Stack Knowledge
as well as HTML,CSS ,Git ,php,javascript,XAMMP Server application
Programming Style : Object Oriented Programming Style for Backend

Mailing Service : PHP mail() function with help of sendmail integrated with Amazon

####--Email a random XKCD challenge--##
This PHP application accepts a visitor’s email address and then verifies the email address with OTP(One Time Password) sent to the visitor's email and after verification random XKCD comics will be sent in every five minutes including the inline image content as well as attachment. User can also Unsubscribe from the email service at any time. Application also contains the Admin Panel to manage all the users in Graphical Interface

##################--Subscription

User will enter his/her email address and then verify the email address with OTP(One Time Password) which will be sent to the visitor's email id and after verification with the correct OTP success message will be displayed on the screen and welcome message will be sent to the visitor's email id. If in case OTP entered by the user is incorrect then Invalid OTP warning will be displayed on the screen. After the successful verification of email id user will get random XKCD comics in mail indox in every 5 minutes. To unsubscribe user can click on the unsubscribe button in mail.


#############----UnSubscribe

User will enter his/her email address and if the email address is not a subscribed email id then Email not found error will be displayed. If the email entered is a subscribed email id, then user will get unsubscribed message on the screen and also an email message to unsubscribe. To subscribe again, user can click on the Subscribe again button link in the email message


#############----Admin Panel


Admin will have to enter the email id and password to login into admin panel. If the email or password is incorrect, then Invalid Credential error message will get displayed. If the email and password is correct, then email containing the OTP(One Time Password) and link will sent to the admin email. OTP and link will be valid only upto 2 minutes and after that they both will expire. If the OTP entered by the admin is incorrect then Invalid OTP error message will be displayed and if OTP entered is correct then user will be redirected to the Admin Home Page and login session will be created for the admin. If the admin will click on the login thorough link, then if link is not expired it will get redirected to the Admin Home Page otherwise after expire it will redirect the admin to the Admin Login Page.

[Note : Very first admin entry by entering email and password after fresh creation of admin table will be considered as default Admin email and password and then for future login only one and same email and password will be used]

[Note : For Assignment testing purpose for mentors, I have formatted the admin table and created a fresh table by running the PHP script]
On Admin home page, total mails sent by the server, total registered users and total active user(subscribed users) will get display, below that all the top 5 users who have received maximum mails will be listed in order and in next table all the last 5 recently added users will get listed.

On the View users tab, admin can view all the users with their status as Un-verified(OTP sent but not verified), Subscribed or Unsubscribed status.

In the Add User tab, admin can add any email id and by default status for that email will be added as a verified/subscribed email. If the email already exists then Email Already exists message will get displayed.

In the Remove user tab, admin can remove the user in one click

In the Edit Details tab, admin can change any user email, total mail sent count as well as status, if any field is empty or does not meet the requirement of valid data, then red color border will be active which indicates the error in particular input field. Drop down will appear if admin wants to change the status of any user. On clicking on save button all the details of that particular user will get updated.

In the Change Password tab, admin has to enter his/her current password, new password and confirm new password, if the current password entry will match with the existing current password then password will get updated otherwise error message will get displayed on the screen.

On clicking the logout tab button, admin will get logged out and all the sessions will get destroyed and admin will redirected to the Admin login page



#####-----Random XKCD comics------#####

Every verified/subscribed user will get random XKCD comics on his/her email id in every 5 minutes, email will contain an attachment along with the inline image as well as comic content. To fetch the comic data, https://c.xkcd.com/random/comic is used programmatically to return a random comic URL which then further sanitize and then use to get all data for content.



## Development

Want to improve? Great! Make the changes and raise a PR. Reach out to me over engtilakchandra@gmail.com
