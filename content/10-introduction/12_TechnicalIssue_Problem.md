---
title: "Technical Issue / Problem" # MODIFY THIS TITLE
chapter: true
weight: 12 # MODIFY THIS VALUE TO REFLECT THE ORDERING OF THE MODULES IF APPLICABLE
---

# The technical hurdles to code, open-source, and containers

## The problem of managing software vulnerabities

Software developers are well-trained professionals that create software applications to solve everyday business and people problems. This software spans a variety of areas, including user interfaces, databases, business logic, and more.  The software developers write is frequently the intellectual property of a company and your development teams write this code with your company's interests in mind.

Software professionals specialize in writing great, functional applications, but not application security.  There are many reasons including the complex nature of how vulnerabilties occur and the sometimes complex exploits needed.  Often times, you can't just visually inspect code and say it is vulnerable.  Most developers would prefer to use a tool designed to identify vulnerabilities.  The alternative is to train every developer on the ever-growing list of vulnerabilities, and techniques to address them.

## The problem of managing Open Source
In industry surveys, Snyk has found that between 70 and 90 percent of a modern application payload is some type of open-source.  This means applications are written and _assembled_.  These open-source dependencies often have their own dependencies, also known as _transitive dependencies_.  One consequence of using open-source software is you have to be aware of the vulnerabilities in the different levels of dependencies.

## The problem of managing Containers
Containers are a wonderful packaging format for shipping modern applications.  Most development teams utilize some form of open-source container image from public repositories, freeing them of the responsibilities of managing the pieces within.  With this flexibility and freedom, you have some of the same problems with of convential open-source software with respect to vulnerabilties.  When we discover a vulnerability in a contain image, the impact is felt by many (sometimes millions) of consumers.

## The problem of managing Code Security
In software development, ensuring code security while maintaining rapid development cycles is a notable challenge. Snyk Code offers a solution to this by providing timely feedback on potential vulnerabilities. Just as modern applications often rely on a mix of custom and open-source components, the code that teams produce can have its own vulnerabilities. With tools like Snyk Code, developers can identify and address these issues in real-time, ensuring that the software is both functional and secure. It underscores the importance of being aware of vulnerabilities at every stage of the development process.

## Next: Who we are
In the next section, we provide an overview of Atlassian and Snyk and how they help teams develop fast and stay secure.
