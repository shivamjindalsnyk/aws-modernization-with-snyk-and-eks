---
title: "Set Up Security in Jira"
chapter: true
weight: 61
---

### Step 1 - Enable the Security in Jira features

Navigate to your Jira Project you want to enable and go to Project Settings > Features > Development > Security and click enable

![Enable Security in Jira Part 1](/images/enable-sij-1.png)
![Enable Security in Jira Part 2](/images/enable-sij-2.png)


### Step 2 - Install the Snyk for Jira App
**Note: You need to be a global Jira admin for this**

Navigate to the Jira Project you enabled with Security and find the new Security tab in the left side. There, click "Connect Tool" > Snyk > "Get It Now". 

Alternatively: You can also navigate to Apps > Find New Apps > Search for "Snyk Security in Jira Cloud. Then Click the app and select "Get it Now"

![Connect Security in Jira Part 1](/images/sij-connect-tool.png)
![Install Security in Jira Part 2](/images/sij-install-tool.png)

### Step 3 - Configure the Snyk Security in Jira App
1. Navigate to the Jira Project you enabled with Security and find the new Security tab in the left side. There, click "Set Up App" 

OR

1. Navigate to Apps > Manage apps in your Jira interface.
2. In the left menu, select Snyk Security in Jira.

After the above:

1. Log in to your existing Snyk account, or sign up for a new Snyk account if you don't have one.
2. In Snyk, select Grant access to allow Snyk to read your Jira Software account information.
3. Select the specific Snyk Organizations you wish to connect to your Jira site, then select Grant app access.


![Configure Security in Jira Part 1](/images/sij-configure-1.png)
![Configure Security in Jira Part 2](/images/sij-configure-2.png)
![Configure Security in Jira Part 3](/images/sij-configure-3.png)

### Step 4 - Link Snyk Scans to Jira Projects
1. Navigate to the Jira Project you enabled with Security and find the new Security tab in the left side. There, click "Finish Set Up" and select Snyk. 
2. Click "Connect security container"
3. Add Snyk Security in Jira as your tool of choice
4. Search for the Snyk Security Scan you want to scan and click "Add"


![Configure Security Scan 1](/images/sij-add-container-0.png)
![Configure Security Scan 2](/images/sij-add-container-1.png)
![Configure Security Scan 3](/images/sij-add-container-2.png)

Next we'll demonstrate how to navigate Security in Jira
