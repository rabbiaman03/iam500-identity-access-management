# Week 6 — Identity Governance: Entitlement Management, Access Reviews and PIM

**Course:** IAM500 — Identity and Access Management  
**Platform:** Microsoft Entra ID Governance (lab tenant)

## Objective

Control **who gets access, for how long, and who checks it**. I bundled resources into a governed catalog (entitlement management), set up a recurring review of group membership (access reviews), and replaced a standing admin role with a **just-in-time** role that has to be activated with MFA and a justification (Privileged Identity Management).

## Lab 22 — Entitlement management: catalogs and resources

Created a **Marketing** catalog for marketing department users. It is enabled internally but not for external users.
![Marketing catalog created next to the built-in General catalog](images/week06-labs/media/image1.png)
*Figure: Marketing catalog created next to the built-in General catalog*

Added resources to the catalog, the **Northwest Sales** group and the **GitHub Enterprise** application, so they can be packaged and requested.
![Adding a group and an application to the catalog](images/week06-labs/media/image2.png)
*Figure: Adding a group and an application to the catalog*

Delegated management by adding **Chris Green as catalog owner**, so the business owner (not IT) manages access to these resources.
![Chris Green added as Marketing catalog owner](images/week06-labs/media/image3.png)
*Figure: Chris Green added as Marketing catalog owner*
![Catalog properties: enabled, not open to external users](images/week06-labs/media/image4.png)
*Figure: Catalog properties: enabled, not open to external users*

Reviewed the Identity Governance access review area at the end of the lab.
![Identity Governance: Access reviews](images/week06-labs/media/image5.png)
*Figure: Identity Governance: Access reviews*

## Lab 25 — Access reviews

Created an access review, **SC300 Access Review Test**, on the Northwest Sales group, so membership is periodically re-certified instead of growing forever.
![Access review created for the Northwest Sales group](images/week06-labs/media/image6.png)
*Figure: Access review created for the Northwest Sales group*

## Lab 26 — Privileged Identity Management (PIM)

Configured the **Compliance Administrator** role so that activation lasts at most **8 hours**, requires **Azure MFA**, and requires a **justification**.
![PIM role settings for Compliance Administrator](images/week06-labs/media/image7.png)
*Figure: PIM role settings for Compliance Administrator*
![Editing the role's activation settings](images/week06-labs/media/image8.png)
*Figure: Editing the role's activation settings*

Made Chris Green **eligible** for the role (not permanently active).
![Eligible assignment of Compliance Administrator to Chris Green](images/week06-labs/media/image9.png)
*Figure: Eligible assignment of Compliance Administrator to Chris Green*
![Assignment settings before saving](images/week06-labs/media/image10.png)
*Figure: Assignment settings before saving*

Signed in as Chris Green: the role appears under **Eligible assignments**, so it gives no privileges until activated.
![Chris Green's eligible role assignment](images/week06-labs/media/image11.png)
*Figure: Chris Green's eligible role assignment*

Activated the role just in time, for 2 hours, with a written justification.
![Activating Compliance Administrator with duration and justification](images/week06-labs/media/image12.png)
*Figure: Activating Compliance Administrator with duration and justification*

Started a second assignment, **User Administrator**, at directory scope.
![Adding a User Administrator assignment](images/week06-labs/media/image13.png)
*Figure: Adding a User Administrator assignment*

## Key takeaways

- **Least privilege over time:** PIM turns standing admin rights into eligible roles that are active only when needed, with MFA, a justification and an expiry. That shrinks the window an attacker can abuse.
- **Delegation:** entitlement-management catalogs let resource owners manage access without making them tenant admins.
- **Recertification:** access reviews catch "access creep" by making owners regularly confirm who still needs access.
- Together these cover the identity lifecycle's governance stage: **request → approve → use → review → remove**.
