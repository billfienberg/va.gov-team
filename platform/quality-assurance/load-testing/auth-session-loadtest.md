# Using authenticated sessions for load testing

## Things you need

1. [Access to internal tools](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/engineering/internal-tools.md) \(specifically Jenkins, but if you have access to one then you tend to have access to all\)
2. [SOCKS proxy access](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/engineering/internal-tools.md#configure-the-socks-proxy)
3. Access to [`devops`](https://github.com/department-of-veterans-affairs/devops) repository
4. A terminal \(For example: Bash, [GitBash](https://gitforwindows.org/), [WSL](https://docs.microsoft.com/en-us/windows/wsl/install-win10), MacOS terminal\)

## Steps to create authenticated sessions

1. Start up the SOCKS proxy
2. Navigate to the [vets-api-load-test-sessions](http://jenkins.vfs.va.gov/job/rake_tasks/job/vets-api-load-test-sessions/) Jenkins task in a browser
3. Log in to Jenkins  

    ![](../../.gitbook/assets/jenkins-login.png)

4. Click "Build with Parameters" from the left side of the site  

    ![](../../.gitbook/assets/jenkins-build-with-parameters.png)

5. Click "Build"  

    ![](../../.gitbook/assets/jenkins-build.png)

6. Click the new build in the list of builds to the left  

    ![](../../.gitbook/assets/jenkins-click-the-build.png)  

7. Select "Console Output" from the menu  

    ![](../../.gitbook/assets/jenkins-console-output.png)

8. Scroll through the output until you see an array of hashes with keys "uuid" and "cookie\_header"  

    ![](../../.gitbook/assets/jenkins-session-cookie-output.png)

9. Copy the entire array, including the lines with square-brackets  

    ![](../../.gitbook/assets/jenkins-session-cookie-output-selected.png)

10. Paste the copied array into a new file and save as `sessions.json`
11. Use the array of session IDs and cookie hashes in `sessions.json` with Python's [JSON library](https://docs.python.org/3/library/json.html)
    * For running a load-test locally \([see Devops Load-Testing README](https://github.com/department-of-veterans-affairs/devops/tree/master/loadtest/README.md)\), save the file into the same folder as your load-test file.
12. Run your load test

