[Back](/en/trouble)
* * *
# Troubleshooting RT Roles and Titles
This is a good article to read if you are having trouble with a function that grants or revokes a role, such as the role panel.

## Can't grant or revoke a role.
## Do you have permissions?
First of all, make sure you have permissions on RT.  
You must have the authority to grant the role.

### Is there a target role below the RT's role?
For example, let's say you have a job title as shown in the image below and you want to put the job title "Notification ON" in the job title panel.  
! [Notifications ON is at the top and RT is at the bottom](/img/trouble/role.jpg)  
This will create a role panel, but no role will be assigned.  
Because RT's "Notifications ON" role is above RT's role, Discord's permissions will fail to grant the role.  
So, in this case, move the RT role above the "Notifications ON" role.

### Redo the role panel
You may think that you've done all the work, but there is a button to get the template in the role panel of RT.  
🛠️Pressing this emoji reaction will send a text to your DM with a command that you can execute to create the same role panel.  
This will allow you to edit it easily.