# Readings: Access Control (ACL)

## [5 steps to simple role-based access control (RBAC)](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)

<!-- ### Author -->

### What is RBAC?

RBAC is nothing more than the idea of assigning system access to users based on their role within an organization. The system needs of a given workforce are analyzed, with users grouped into roles based on common job responsibilities and system access needs. Access is then assigned to each person based strictly on their role assignment. With tight adherence to access requirements established for each role, access management becomes much easier.

The question therefore is why, with an achievable and time-honored approach, we can’t seem to get a handle on access control. We are certainly being pushed in that direction of RBAC, with all of the major standards, including PCI DSS, HIPAA and Gramm-Leach-Bliley all requiring some form of it.

I would suggest that one reason RBAC is not used more frequently is that for small to medium sized companies, it seems easier to just do this on an ad-hoc basis as each employee joins the company. The challenge is that with as many permutations as can exist with just a few systems involved, the approach becomes unsustainable.

### Benefits of RBAC?

With the proper implementation of RBAC, the assignment of access rights becomes systematic and repeatable. Further, it is much easier to audit user rights, and to correct any issues identified.

RBAC may sound intimidating, but it can in reality be easy to implement, and will make the ongoing management of access rights much easier and more secure.

The data breach you prevent may be your own.

### RBAC implementation 
Hopefully I have convinced you to take a closer look at RBAC. If so, consider the following simplified five-step approach to getting it implemented:

1. Inventory your systems

    Figure out what resources you have for which you need to control access, if you don't already have them listed. Examples would include an email system, customer database, contact management system, major folders on a file server, etc. 

2. Analyze your workforce and create roles

    You need to group your workforce members into roles with common access needs.  Avoid the temptation to have too many roles defined. Keep them as simple and stratified as possible.

For example, you might have a basic user role, which includes the access any employee would need, such as email and the intranet site. Another role might be a customer service rep, that would have read/write access to the customer database, and a customer database administrator, that would have full control of the customer database. 

3. Assign people to roles

    Now that you have a list of roles and their access rights, figure out which role(s) each employee belongs in, and set their access accordingly. 

4. Never make one-off changes

    Resist any temptation to make a one-off change for an employee with unusual needs. If you begin doing this, your RBAC system will quickly begin to unravel. Change the roles as required or add new ones when really necessary. 

5. Audit

    Periodically review your roles, the employees assigned to them, and the access permitted for each. If you discover, for example, that a role has unnecessary access to a particular system, change the role and adjust the access level for all employees in that role. 

    As an example, many healthcare organizations, given the need for regulatory compliance in controlling access to medical records, use RBAC to define exactly what access to medical records each type of clinician may need.  While a doctor might have almost unlimited access to the records of patients he/she manages, a receptionist might be limited to basic contact information needed to manage appointments.  Given the large number of staff members in well stratified roles, RBAC is an efficient way to control record access in compliance with HIPAA, and other regulations.

    There are tools that can help with setting up RBAC. Many systems, such as Microsoft Active Directory, have built in roles that you can use as a starting point, which you can extend to fit your unique situation. You can also use an identity management system to automate the assignment of privileges based on role. 









---

[Back to Home](https://pdariuslee.github.io/reading-notes/)