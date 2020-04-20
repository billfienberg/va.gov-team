# Integrate TestRail with GitHub

_Preconditions: You have a GitHub account and a TestRail account._

1. Navigate to your GitHub [personal access tokens page](https://github.com/settings/tokens).
2. Use the "Generate new token" button to create a new access token for personal TestRail integration.
3. Add a meaningful note for the token.

   ![](../../.gitbook/assets/token-note.png)

4. Select an appropriate scope for the token.  Since defects and user stories should be stored in **va.gov-team** which is a public repository, it is sufficient to select the "public\_repo" scope.

   ![](../../.gitbook/assets/token-scope.png)

5. Use the copy button next to your token to store it in your clipboard.

   ![](../../.gitbook/assets/token-copy.png)

6. Navigate to your [TestRail My Settings](https://dsvavsp.testrail.io/index.php?/mysettings) page.
7. Click the Settings tab at the top of the page.
8. Populate the GitHub User input box with your GitHub username.
9. Populate the GitHub Password input box with the GitHub token stored in your clipboard. 

   !\[TestRail token my settings\]\[testrail-token-mysettings\]

10. Click the Save Settings button.
11. Done!

\[testrail-token-mysettings\]: ../images/testrail-tutorials/token-mysettings.png

