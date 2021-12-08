# Using Real Time Collaboration feature in Datahub

[Real-Time Collaboration in Jupyter](https://github.com/jupyterlab/rtc) is one of the most requested functionalities, which has also proven to be a complex use case to develop. However, due to the [generous contribution](https://github.com/jupyterlab/rtc/graphs/contributors) from various open-source contributors, this experimental functionality is enabled in a few hubs (Data 8 and D-Lab at the time of write-up). So, if you are interested in enabling this functionality in your respective hub, please check with the hub admins. 

After that, You can start collaborating with others by following the below steps,

# Step 1

Open your IPython (ipynb) notebook files in Jupyter Lab or Retro Lab interface. If you are unsure how to generate a nbgitpuller link to access your notebook in Jupyter Lab or Retro Lab interfaces, Please install this [plugin](https://addons.mozilla.org/en-US/firefox/addon/nbgitpuller-link-generator/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search) in the Mozilla Firefox browser, which will walk you through the steps required to generate the link for the file easily.

```{warning}
Keep in mind that Real-Time Collaboration(RTC) functionality is not enabled in classic notebook.
```

# Step 2
As a next step, Generate the shareable link to be shared with your collaborators. Follow the below steps to generate this link,
- In the Menu bar, Click on the Share option (option next to Help). 
- Select "Share Jupyter Server Link" which opens a prompt a the centre of the screen that shows an option to copy the shareable link. 
- Select "Copy Link" option which copies the link to your clipboard

```{figure} ../images/Share_link.gif
:width: 500px
:align: center
:name: Shareable Link

Here is how you can generate a shareable link
```

# Step 3
Share this link with your collaborators. They will be able to access your notebooks immediately and make edits to the notebook in real-time.
You can also see the cursors from other users with an anonymous username, a username that will disappear in a few seconds to make room for what is essential, the document’s content.

```{figure} ../images/RTC_demo.gif
:width: 500px
:align: center
:name: RTC Demo

Real Time Collaboration (RTC) in action
```

If you are interested to learn more about how real time collaboration works in Jupyter Lab, do refer to this [documentation](https://jupyterlab.readthedocs.io/en/stable/user/rtc.html)
If you are interested to get under the hood of real time collaboration and understand the framework enabling the shared data type, do refer to this [documentation](https://github.com/yjs/yjs)