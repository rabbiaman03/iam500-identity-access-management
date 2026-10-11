# Week 1 — Entra ID Users, Tenant Settings and Groups

**Course:** IAM500 — Identity and Access Management  
**Platform:** Microsoft Entra ID / Azure (lab tenant)

## Objective

Set up the foundations of a Microsoft Entra ID tenant: delegating admin roles, provisioning users in bulk, assigning licenses, adding a custom domain, configuring tenant privacy details, and building static and dynamic groups.

## Lab 01 — Users and role delegation

Before any role was assigned, the new user signed in but could not manage enterprise applications — showing least privilege by default.

![New user signed in without application-management rights](images/lab01/media/image1.png)
*Figure: New user signed in without application-management rights*

Assigned the user an application-administration role in Entra ID; the user could then create an enterprise application.

![Role assigned to the new user](images/lab01/media/image2.png)
*Figure: Role assigned to the new user*

Created several users at once with the Bulk create CSV upload.

![Bulk user creation completed](images/lab01/media/image3.png)
*Figure: Bulk user creation completed*

Assigned a Windows 10 license to the user.

![Windows 10 license assigned](images/lab01/media/image4.png)
*Figure: Windows 10 license assigned*

## Lab 02 — Tenant configuration

Added a custom subdomain to the tenant.

![Custom subdomain added](images/lab01/media/image5.png)
*Figure: Custom subdomain added*

Set the tenant's privacy contact and privacy statement URL.

![Privacy contact configured](images/lab01/media/image6.png)
*Figure: Privacy contact configured*

![Privacy statement saved](images/lab01/media/image7.png)
*Figure: Privacy statement saved*

## Lab 03 — Groups

Created a security group for access control.

![Security group created](images/lab01/media/image8.png)
*Figure: Security group created*

Created a Microsoft 365 group for collaboration.

![Microsoft 365 group created](images/lab01/media/image9.png)
*Figure: Microsoft 365 group created*

Created a dynamic group whose membership rule automatically includes all users.

![Dynamic group with an all-users rule](images/lab01/media/image10.png)
*Figure: Dynamic group with an all-users rule*

## Key takeaways

- Role-based access control: users get no admin rights until a role is assigned.
- Bulk operations and dynamic membership rules cut manual identity work.
- Security groups control access; Microsoft 365 groups add collaboration resources.
