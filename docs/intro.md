---
sidebar_position: 1
---

# Getting Started

Let's discover **BotShard**.

## 1. Creating a server

Get started by **[creating an account](https://dashboard.botshard.com/)**.

Click **Servers** in the sidebar and **Create a Server**.

![Create Server](/img/dashboard_create.png)

Select a server name, location and language:

> If you are planning on running Python, select **`python generic`**;
>
> If you are planning on running Node.js, select **`nodejs generic`**;
>
> And so on.

After creating a server, click **Manage** button at the bottom.

![Manage Server](/img/dashboard_manage.png)

## 2. Introducing... the Panel

You should be redirected to **[the panel](https://panel.botshard.com/)**. If asked, login using the same credentials as your dashboard account.

You are now in the control panel for your server!

![Panel Overview](/img/panel_console.png)

Lets have a small overview of panel sections.


### Console

You will be able to view the general information about your server, along with its console output. This is also the place to start, stop, and restart your server.

:::tip

Here, you will be able to find your server UUID, node, IP and other information which might be helpful when asking for support.

:::

:::caution

Despite its look, "Type a command" field is dedicated for I/O input into your program, such as when asked by the `input()` function from Python.

:::


### File Manager

![File Manager](/img/panel_file_manager.png)

In this tab, you will be able to manage your files, upload new ones, edit them, archive, rename, and more.


### Startup

![Startup](/img/panel_startup.png)

This tab allows you to change the values used by BotShard when running your bot.


## 3. Setting up your bot

### Uploading files

#### Using Git

Go to **[Startup Tab](#startup)** and change **Git Repo Address** to your Git repository link. You can also change the **Git Branch**, **Git Username**, and **Git Access Token** if nessecery. Make sure to enable **Auto Update** or it won't pull the files.

#### Manually

Go to **[File Manager](#file-manager)** and upload your files.

As uploading folders is not supported, the recommended way to transfer your files is to archive them into a **.zip** file and upload that.

After doing so, click **...** and select **Unarchive** to extract the archive.

![Unarchive](/img/panel_file_options.png)


### Installing packages

The next step is to install nessecery packages to start the bot, such as `discord.py`, `discord.js`, `nextcord`, or any others.

If you don't have any required packages or you are using language without them (i.e. Java), skip this step.

#### Automatically

The packages will install automatically if provided with `requirements.txt` file on Python or `packages.json` on Node.

#### Manually

Go to **[Startup Tab](#startup)**, locate **Additional Packages** field and put all your package names, separated by spaces.

![Additional Packages](/img/panel_additional_packages.png)

:::danger No

`pip install discord.py`

`npm i`

`discord.py, flask`

`discord.pyflask`

`discord.py random` (**random** is a built-in module!)

:::

:::tip Yes

`discord.py flask`

:::


### Change startup file

By default, the files run by BotShard are:

- `app.py` for Python

- `index.js` for Node

- `sneakyhub.jar` for Java

- ...

If those names don't match with your main file, you will need to either rename the file itself in **[File Manager](#file-manager)** or go to **[Startup Tab](#startup)** and change the filename there.

![Change the Startup File](/img/panel_app_py_file.png)


## 4. Testing - does it work?

Finally, head to the **[Console](#console)** and click **Start**.

If everything works, hoooray!!! 🥳🥳

Make sure to open the **[dashboard](https://dashboard.botshard.com/)** every 2 days or your server will get suspended. (**[Learn Why](common-issues/suspended)**)


### If it doesn't...

Click **Next** button down below to see some common issues you might face!
