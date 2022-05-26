# Shiny

[Shiny](https://shiny.rstudio.com/) is a R package which makes it easy to build interactive web apps. R shiny server in Datahub is used to build interactive dashboards. Here is a short demo of a shiny application below,

```{figure} ../images/shiny_combined.gif
:width: 500px
:align: center
:name: Shiny Demo

Short Demo to launch Shiny application in Datahub
```

If you are interested to explore Shiny application further then you can play with examples from this [Github repository](https://github.com/rstudio/shiny-examples) and [few other examples](https://github.com/gastonstat/shiny-introstats/) created by a stats faculty. Here are couple of approaches you can take to launch a shiny application,

**Approach I:**
- Install the nbgitpuller plugin in [Google Chrome](https://chrome.google.com/webstore/detail/nbgitpuller-link-generato/hpdbdpklpmppnoibabdkkhnfhkkehgnc)/[Mozilla Firefox](https://addons.mozilla.org/en-US/firefox/addon/nbgitpuller-link-generator/) browser.
- Upload the Shiny application to Github or choose an example from existing applications.
- Select the application home directory and choose the option "shiny" from the nbgitpuller plugin.
```{figure} ../images/launchshinyapp.PNG
:width: 500px
:align: center
:name: Shiny via nbgitpuller link

Launch Shiny application via nbgitpuller plugin
```
- Paste the link in a browser to access the shiny application. Here is an example [link](https://datahub.berkeley.edu/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Frstudio%2Fshiny-examples&branch=main&urlpath=shiny%2Fshiny-examples%2F003-reactivity%2F).

**Approach II:**

- Clone the [GitHub repository](https://github.com/rstudio/shiny-examples) with Shiny examples in your instance of Jupyterhub.
- Launch the Shiny server.

```{figure} ../images/launchshiny.PNG
:width: 500px
:align: center
:name: Shiny

Short Launch Shiny
```

- Point the Shiny server to an example from the cloned repository.
- Explore the rendered example as part of the shiny dashboard.

```{figure} ../images/shinyDashboard.PNG
:width: 500px
:align: center
:name: Shiny Dashboard

Explore Shiny Dashboard
```

You can also view the code that generated the dashboard as part of the rendered output. 

```{figure} ../images/shinycode.PNG
:width: 500px
:align: center
:name: Code for Shiny

Code that generates Shiny dashboard
```