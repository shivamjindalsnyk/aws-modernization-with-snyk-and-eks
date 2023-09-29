---
title: "Navigating Security in Jira"
chapter: true
weight: 62
---

# Manage Security Vulnerabilities in Jira
After the installation and configuration of the Snyk Security in Jira Cloud app, vulnerabilities can be viewed on the security tab of the Jira project page.

## Viewing Vulnerabilities:

1. Navigate to the Vulnerabilities section on the security tab.
2. Snyk displays the severity, status, and identifiers of the vulnerabilities.
3. Click on the title to open the details in Snyk Web UI.

![View Issues in Security in Jira](../images/view-issues-jira.png)


## Searching, Filtering, and Sorting Vulnerabilities:

1. Utilize the search bar and filters in the Vulnerabilities section to customize the vulnerability list to show those relevant to your Organization.
2. By default, ignored and closed vulnerabilities are hidden, but can be viewed using the Vuln. status filter.
3. Click on the title of a column to sort vulnerabilities by that attribute.


## Creating a Jira Issue from a Vulnerability:

1. During the triage process, add a Jira issue to the sprint or backlog to ensure that the necessary work for resolving the vulnerability is planned and tracked.
2. Navigate to the Snyk Security tab, find a vulnerability, and click Create issue.
3. Snyk provides comprehensive vulnerability information to Jira, aiding users in resolving issues.

![Create Issues in Security in Jira](../images/sij-create-issue.png)

## Linking an Existing Jira Issue to a Vulnerability:

If a Jira issue already exists for a vulnerability, link the vulnerability to the existing Jira issue.
Click the three dots in the Actions column next to the vulnerability and select Link issue.
