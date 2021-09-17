# Hub Admin Privileges

```{note}
Curious about what privileges admins have in Datahub? If yes, read below!

```

**What does admin access in the hub mean?** 

Admin feature provides the necessary access required to support students using your hub. If you are an admin user, you have access to the following features,

1. You can start and stop the students' server in your dedicated hub
2. You can access the student server to debug issues in their instance

```{warning}
Admin privileges are hub-wide. If you're a teaching team member who happens to be also a student in another course on the same hub, then there can be a conflict of interest.
```

Check this image to know your privileges for the admin option

```{figure} ../images/admin.png
:width: 500px
:align: center
:name: Datahub Admin

Here is how the admin dashboard looks like!
```
```{note}
If you are an undergrad student you'll not get admin access in any non-course-specific datahub
```

**How do I get access to the admin option?** 

We generally recommend **only** the teaching team to have admin access. If you are part of the teaching team and require admin access, please create a request using this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=admin_request.yml)

**How do I navigate the admin portal?**

If you have admin access and want to know how to access admin portal then use the following steps,

- Login to your hub instance
- Click the admin option from the top bar

```{figure} ../images/adminaccess.PNG
:width: 500px
:align: center
:name: Datahub Admin snapshot

Here is where you can find admin option!
```
- Once  you click, you have access to instances of users and admins in that specific hub

```{note}
If you are using the R hub, then you may need to follow the below steps,

- You can replace https://r-staging.datahub.berkeley.edu/user/your-calnet-id/rstudio/ with https://r-staging.datahub.berkeley.edu/hub/admin to access the admin interface.
- You can use https://r-staging.datahub.berkeley.edu/hub/home to restart your server.
```

**How do I start a student server?**

- Click on the control panel

```{figure} ../images/controlpanel.PNG
:width: 500px
:align: center
:name: Control Panel

Here is how the control panel option looks like!
```
- Click admin option

```{figure} ../images/adminaccess.PNG
:width: 500px
:align: center
:name: Datahub Admin snapshot

Here is where you can find admin option!
```
- Find the user whose server you want to restart. 

```{figure} ../images/user.PNG
:width: 500px
:align: center
:name: User List

Here is how to search for an user!
```
- Click restart server option

**How do I stop a student server?**

- Click the control panel option
- Click admin option
- Find the user whose server you want to stop. 
- Click stop server option

**How can I access the instance of a student server?**

- Click the control panel option
- Click admin option
- Search the calnet id of the student's instance you want to access
- Click access server option to access student's instance


```{figure} ../images/accessserver.PNG
:width: 500px
:align: center
:name: Access Server

Here is how to access a server's instance!
```
