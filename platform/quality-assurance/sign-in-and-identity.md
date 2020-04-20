# Quality Assurance of Sign-in and Identity

To sign in to vets.gov you need either an ID.me, MHV, or DS Logon account. Each of these providers will then pass a SAML response back that includes various user specific attributes. These attributes will always include `email, uuid, and level of assurance.` Depending on the level of assurance, additional attributes may be available, but these additional attributes will vary depending on the sign-in partner.

CAN we list out what gets passed in SAML response for each sign in partner or link to where this information lives?

To sign in you should do the following: 1. Go to [https://staging.vets.gov](https://staging.vets.gov) 2. If prompted for HTTP basic auth username and password you can use `veterans:am3rica` 3. Click on "Sign In" in the upper right hand corner. An overlay should appear with the various sign in methods. 4. Follow any of the steps below for various test scenarios to test Sign-in and Identity. 5. Before every test scenario, make sure to sign out and close the tab and create a new tab for testing!

## ID.me

### Create an ID.me LOA1 without MFA

1. Click "Create an ID.me account" and a modal window should appear.
2. For email, if you have a gmail account, you should enter a variation of your personal email address as follows: 

   `kam+idmeLOA1_noMFA_1@adhocteam.us`

3. You might want to keep track of these accounts and their account states for future testing.
4. Enter password and password confirmations. Use `Tester1$` as the password.
5. Check the box accepting ID.me T&Cs  
6. Click the button to continue with account creation.
7. You should verify that you received two emails: "Welcome to ID.me" and "Your ID.me email confirmation code"
8. On staging, the next modal window will include the confirmation code pre-populated for you. So just click continue.
9. On the next screen you are prompted for adding MFA account. For this step test we are SKIPPING MFA, scroll down, and select "No, I do not want to secure my account at this time."
10. You should now be signed in as an LOA1 ID.me user without MFA. Your email should appear in the upper right corner.
11. In the future you should be able to test with this account if you wish to test this particular flow. If you want to test the actual flow itself you can repeat the steps above.
12. Click on your email address and a dropdown should appear. Select "Account." If you select the email at the top right it should bring you to account/profile page.  On account/profile it should show that you have not verified your account and you have not setup 2fa. 

### Create an ID.me LOA1 with MFA added later

1. Click "Create an ID.me account" and a modal window should appear.
2. For email, if you have a gmail account, you should enter a variation of your personal email address as follows: 

   `kam+idmeLOA1_MFAlater_1@adhocteam.us`

3. You might want to keep track of these accounts and their account states for future testing.
4. Enter password and password confirmations. Use `Tester1$` as the password.
5. Check the box accepting T&C
6. Click the button to continue with account creation.
7. You should verify that you received two emails: "Welcome to ID.me" and "Your ID.me email confirmation code"
8. On staging, the next modal window will include the confirmation code pre-populated for you. So just click continue.
9. On the next screen you are prompted for adding MFA account. For this step test we are SKIPPING MFA, scroll down, and select "No, I do not want to secure my account at this time."
10. You should now be signed in as an LOA1 ID.me user without MFA. Your email should appear in the upper right corner.
11. Click on your email address and a dropdown should appear. Select "Account."
12. On your account/profile page, scroll down and you should see a yellow warning banner. Click on "Add Security step."
13. A modal should appear. Select "Text Message or Phone Call."
14. Enter your phone number. Make sure that "Text" is selected. And Click "Continue."
15. On staging the confirmation dialog should be pre-populated. Click "Continue."
16. You should see a prompt saying "Your account is now secure."
17. Click "Continue" and you should be signed in still, with MFA now enabled.
18. You should land back on the "Account" page and verify that the yellow banner is no longer visible.  You should also see a link to verify your identity because this account is not identity proofed. 
19. You can verify that MFA is now required on this account by signing out and signing back in. You may choose to use this account for future testing, but if you wish to test the flow, you will need to produce the above steps again.

### ID.me LOA1 verified to LOA3 NOT IN MVI.

...

### ID.me LOA1 verified to LOA3 in MVI

...

## MHV

### MHV Basic Account

...

### MHV Advanced Account

...

### MHV Premium Account

...

## DS Logon

### DS Logon LOA1 Account

...

### DS Logon LOA2 Account

...

### DS Logon LOA3 Account

