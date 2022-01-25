# Use Realtime file sharing using SyncThing

Are you a student interested in collaborating with fellow students in a team project? or an instructor who needs to share assignment solutions/course materials with your teaching team that isn't released to students? Datahub currently allows this Dropbox-like functionality to share selected file(s)/folder(s) with collaborators by using a third-party application called [SyncThing](https://syncthing.net/). SyncThing allows users in a hub to create a folder that can be shared with collaborators either part of the same hub or across different hub(s). 

Refer to the below steps to learn how to use SyncThing as part of your workflow,

# Step 1
- Login to your hub's tree. 
- Click on the "New" option in the dropdown list 
- Select "Syncthing" option from the list 

```{figure} ../images/syncstep1.PNG
:width: 500px
:align: center
:name: Selecting SyncThing

Here is how you launch SyncThing application
```

# Step 2
- Request device id from your collaborator(s) who needs access to this shared folder.
- Collaborators can identify their Device ID by clicking on "Actions -> Show ID" option in their SyncThing account.

```{figure} ../images/syncstep1.2.PNG
:width: 500px
:align: center
:name: Show Device ID

Here is how you can identify the device id for your device
```

- Find and click "Add Remote Device" option. To add collaborators, Paste your collaborator's Device ID in the shown prompt.

```{figure} ../images/syncstep1.1.PNG
:width: 500px
:align: center
:name: Add Remote Device

Here is how you can add a remote device to your shared folder
```

# Step 3
- Check whether the devices are synced by looking at the available devices
- If yes, Create a folder where you want to upload all your content and share with your collaborators. 
- Select the "Add Folder" option to create a folder. 
- Click the "Sharing" tab and from the listed devices and select the device to which you want to share this folder.

```{figure} ../images/syncstep4.PNG
:width: 500px
:align: center
:name: Share Folder

Here is how you can share a folder with your collaborator(s)
```

If your collaborator wants to provide access to a folder, you need to share your device id. Once they are able to add your device id to the shared folder, you will receive a notification like the one shown below,

```{figure} ../images/syncstep3.PNG
:width: 500px
:align: center
:name: Notification

Here is how you will receive a notification when a collaborator adds you to a shared folder
```

Finally, Here is a short GIF that walks you through the entire process to set up realtime file sharing using SyncThing in a step by step manner.


```{figure} ../images/syncthingdemo.gif
:width: 500px
:align: center
:name: File Sharing Demo

Demo of SyncThing!
```
