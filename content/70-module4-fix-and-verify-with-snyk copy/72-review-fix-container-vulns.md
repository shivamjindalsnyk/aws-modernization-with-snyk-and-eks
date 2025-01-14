---
title: "Review and Fix Container Base Image Vulnerabilities in Snyk"
chapter: true
weight: 72
---

# Overview
As previously mentioned, Snyk scans Containers to identify vulnerabilities in both the Container Base Image and the Application Manifests inside. In this step we'll review the vulnerabilities in the base image to pick a more secure base image for our container.  

### Step 1 - Review the ECR Base Image scan results
Let's start by reviewing the vulnerabilities introduced into the Container from the Base Image. In the newly imported ECR project, click into Base Image by selecting the Debian project.

Same as before, the Issues show an Issue Card for each Vulnerability, organized by Snyk's Priority Score. Unique to Containers is the Panel at the top that shows Base Image Recommendations. These are broken up by Minor, Major, or Alternative depending on the version change.

### Step 2 - Apply a more Secure Base Image
This time we'll use the Cloud9 IDE to act on the guidance provided by Snyk. In Cloud9, find the Dockerfile that contains the instructions to build the Container Image. The current Base Image is specified in its FROM statement.

We can apply a more secure base image by updating this line in the Dockerfile. Go ahead and change `node-xxx` to the minor upgrade `node-xxx`. We apply a minor upgrade to minimize the chances of introducing a breaking change.

### Step 3 - Push the Changes to Bitbucket
Once applied, save the Dockerfile, then commit your changes to Bitbucket using `git push`. 

```sh
git push
```

In real life, you likely wouldn't commit changes directly to your repo's main branch in this way. You would probably use a new branch, test the container locally, and do many other steps to prevent breaking changes.

### Step 4 - Verify the Fix
Once Merged, your Bitbucket Pipeline will run to re-build and push the Container Image. This will take a few minutes. When the Snyk tests run, the Pipeline Execution output will show a container with significantly less vulnerabilities than when it ran previously.

Once the Container is pushed to ECR, import the newly built container image tag like you did before to see a reduction in vulnerabilites in the ECR-imported project.

Starting with a more secure base image before tackling vulnerabilities in individual packages is a great way to greatly reduce the number of vulnerabilities that must be triaged.
