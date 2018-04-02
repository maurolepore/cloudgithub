Connecting rstudio.cloud and GitHub
================

-   [On rstudio.cloud](#on-rstudio.cloud)
    -   [Login to rstudio.cloud and create a new project from git repo](#login-to-rstudio.cloud-and-create-a-new-project-from-git-repo)
    -   [View link (remote origin) between rstudio.cloud and GitHu](#view-link-remote-origin-between-rstudio.cloud-and-githu)
    -   [If necessary, update remote origin](#if-necessary-update-remote-origin)
    -   [Tools &gt; Global options &gt; Git &gt; Create key](#tools-global-options-git-create-key)
    -   [View and copy public key](#view-and-copy-public-key)
-   [On GitHub](#on-github)
    -   [Give SSH key to GitHub](#give-ssh-key-to-github)
    -   [If necessary configure git](#if-necessary-configure-git)

On rstudio.cloud
================

Login to rstudio.cloud and create a new project from git repo
-------------------------------------------------------------

![](https://i.imgur.com/E1wcTup.png)

View link (remote origin) between rstudio.cloud and GitHu
---------------------------------------------------------

View remote

``` bash
git remote -vv
```

If necessary, update remote origin
----------------------------------

Remove remote

``` bash
git remote remove origin
```

Add remote

``` bash
git remote add origin git@github.com:OWNER/REPONAME.git
git push -u origin master
```

Tools &gt; Global options &gt; Git &gt; Create key
--------------------------------------------------

![](https://i.imgur.com/8cyFyn7.png)

View and copy public key
------------------------

On GitHub
=========

Give SSH key to GitHub
----------------------

<https://github.com/settings/keys>

![](https://i.imgur.com/Zu1SmoB.png)

If necessary configure git
--------------------------

To paste text in the terminal use Shift + Insert.

``` bash
git config --global user.email "USEREMAIL@gmail.com"
git config --global user.name "USERNAME"
```
