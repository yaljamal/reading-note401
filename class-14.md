# RBAC
 * In computer systems security, role-based access control (RBAC) or role-based security is an approach to restricting system access to authorized users. It is used by the majority of enterprises with more than 500 employees and can implement mandatory access control (MAC) or discretionary access control (DAC).

# Access Controls (ACL)

A CMS might …

* Allow *admin* users to create categories, content, manage user accounts, and run reports
* Allow *editor* users to create, edit and delete existing content, but not see or manage user accounts
* Allow *guest* users to access (read) content
* Allow *user* users (logged in users) to access (read) content and apply a thumbs-up/down to content, but not change the actual content

* Back End (API Layer) can do:
1. Manage the login cycle with the front-end application
2. Maintain the User’s database
3. Maintain roles for each user
4. Authenticate users (basic and bearer)
5. Create, manage, and apply Role Based Access Controls
6. Maintain and reference their capabilities, based on their role
7. Restrict access to features (like routes) based on capabilities

* Express Middleware could be used to restrict access to routes
* Mongoose Middleware/Hooks could be use to restrict access to business logic

* Front End (Client Layer) can do:
1. Initiate the login process
2. Store login tokens as cookies
3. Manage login state, capabilities
4. Control physical & visual access (hide/show/alter) to components based on RBAC rules
5. Alter behaviors based on RBAC rules

* What is RBAC?
*  is nothing more than the idea of assigning system access to users based on their role within an organization.

* RBAC implementation
2. Inventory your systems
3. Analyze your workforce and create roles
4. Assign people to roles
5. Never make one-off changes
6. Audit
