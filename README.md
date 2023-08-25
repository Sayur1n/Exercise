# Tutorial: Create a Lip Tooth
This is the first part of a tutorial that introduces a few fundamental features of Lip. If you're just getting started with Lip, be sure to take a look at [Getting Started](https://docs.lippkg.com/en/quickstart.html) and [Creator's Guide](https://docs.lippkg.com/en/creator_quickstart.html), which introduces the basic commands of Lip.

In this tutorial you'll create a tooth containing a plugin of LiteLoaderBDS.
## Prerequisites
+**Some project management experience.** You ought to learn the basic usage of Git, and the basic syntax of JSON in advance.
+**A tool to edit tooth.json** Any text editor you have will work fine. The most popular are VSCode and Vim.
+**A command terminal** Lip works well with both PowerShell and cmd in Windows.
+**Lip command-line tool** You should install Lip in advance. For more information, refer to [Installation](https://docs.lippkg.com/en/installation.html)

## Prepare plugin distributions
Lip fetches all content of a version of a Git repository for installing. Therefore, you should get all files to be installed ready under the management of Git.

If you just work with text (e.g. script plugins, addons), you could just use the repository for development to create a tooth.

However, if you are working with binaries (e.g. native plugins, worlds), you might have to create another repository to store the content. Otherwise, the binaries may make your repository too large to manage.

In this example, we assume the repository structure as listed below:
'''
exampleplugin.dll
exampleplugin/
  config.json
  libexample.dll
  data/
'''

## Initialize the tooth
1.Open a command prompt and cd to the repository root. If you are using Windows, you can just press shift and right click in the file explorer, then click "Open PowerShell window here".
2.Run the command below to initialize the tooth. The command will create a tooth.json under the root of the repository.
'<font color=red>shell'
   'lip tooth init</font>'




   
