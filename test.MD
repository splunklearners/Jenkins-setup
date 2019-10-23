# Integrate Jenkins project with Github reposistory


let's configure the GitHUb and Jenkins integration. Let's begin with the GitHub side!

### steps

```
Step 1: Go to your GitHub repository and click on Settings.
Step 2: Click on Webhooks and then click on Add webhook.
Step 3: In the Payload URL field, paste your Jenkins environment URL. At the end of this URL, add /github-webhook/. (ex: http:17.25.65.32:8080/github_webhook/)
        In the Content type select application/json and leave the Secret field empty.
Step 4 :In the 'Which events would you like to trigger this webhook?' section, choose Let me select - "just the push event". then select "Add Webhook"

```

### We're done with the configuration on GitHub's side! Now, let's move on to Jenkins.

```

Step 5: In Jenkins, click on New Item to create a new project.
Step 6: Give your project a name, them choose Freestyle project and finally, click OK.
Step 7: Click on "GitHub project" and enter you Github repository url ( not url with .git extenstion)
Step 8: Click on the Source Code Management tab.
Step 9: Click on Git and paste your GitHub repository URL in the Repository URL field. ( with .git extenstion)

```
That's it! Your GitHub repository is integrated with your Jenkins project. 
You can now update or change any of the files found in the GitHub repository and trigger the Jenkins job to run with every code commit.
