# Week 5 — App Registrations, Enterprise Apps and API Permissions

**Course:** IAM500 — Identity and Access Management  
**Platform:** Microsoft Entra ID / Azure (lab tenant)

## Objective

Register applications with the Microsoft identity platform, expose an API with scopes, assign users to enterprise apps, and grant admin consent for API permissions.

## Lab 19 — App registration

Registered the demo application.

![Registered app](images/week05-labs/media/image1.png)
*Figure: Registered app*

Configured the redirect URI.

![Redirect URI configured](images/week05-labs/media/image2.png)
*Figure: Redirect URI configured*

Set the Application ID URI.

![Application ID URI saved](images/week05-labs/media/image3.png)
*Figure: Application ID URI saved*

Exposed an API scope.

![Scope added](images/week05-labs/media/image4.png)
*Figure: Scope added*

Tried to create a custom role. *Custom roles need Entra ID P1/P2, which the lab tenant did not have.*

![Custom role creation](images/week05-labs/media/image5.png)
*Figure: Custom role creation*

## Lab 20 — Enterprise applications

Created an enterprise application.

![Enterprise app created](images/week05-labs/media/image6.png)
*Figure: Enterprise app created*

Assigned a user to it.

![User assigned](images/week05-labs/media/image7.png)
*Figure: User assigned*

## Lab 21 — Permissions and consent

Granted tenant-wide admin consent.

![Admin consent granted](images/week05-labs/media/image8.png)
*Figure: Admin consent granted*

Added API permissions.

![Permissions added](images/week05-labs/media/image9.png)
*Figure: Permissions added*

## Key takeaways

- App registration defines the app's identity; the enterprise app (service principal) controls who can use it in the tenant.
- Scopes and admin consent enforce least privilege for APIs.
