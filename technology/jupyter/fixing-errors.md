# Fixing JupyterHub Errors

You may run into different types of errors when you are using the JupyterHub. One common error is a Jupyter notebook becoming unresponsive. Another type of error is a user not being able to access some part of their JupyterHub account.

We have outlined two methods below that you should try for each error type. For errors related to execution of code, such as the notebook not running properly, you should try restarting the kernel. For errors related to access, you should try restarting the server. If these methods do not solve the issue you are facing, please [post on Piazza](http://piazza.com/berkeley/other/cs97).

## Restarting the Kernel

If your notebook becomes unresponsive, you can try to restart the kernel.

![](/assets/restart-kernel.png)

## Restarting Servers

There are different methods for restarting your own and restarting another user's server.

### Restarting Your Own Server

All users can restart their own servers. To do so, start by going to the control panel.

![](/assets/control-link.png)Click the `Stop My Server` button.

![](/assets/stop-my-server.png)Once the server has stopped and the `Stop My Server` button is no longer visible, click the `My Server` button to restart the server.

![](/assets/start-my-server.png)

### Restarting Student Servers

Users with admin privileges on DataHub can restart other users' servers. To restart a student's server, first go to the control panel.

![](/assets/control-link.png)Click on the `Admin` button at the top of the page. If you do not see this button, you do not have admin rights. To request admin rights, please [post on Piazza](http://piazza.com/berkeley/other/cs97).

![](/assets/admin-link.png)After clicking the `Admin` button, you will see the admin panel. Usernames have been obfuscated here. To search for a user, you can use find \(type Control+F or Command+F\). An individual's username is the same as their CalNet ID. When you have found the desired user, click the `stop server` button in the user's row.

![](/assets/admin-panel.png)

After clicking the `stop server` button, you can click the `start server` button in the user's row.

