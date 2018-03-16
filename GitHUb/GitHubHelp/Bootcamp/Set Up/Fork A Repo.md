## Fork A Repo

分拣回购

MAC WINDOWS LINUX

A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project.

一叉是一个仓库的副本。分拣存储库允许您在不影响原始项目的情况下自由尝试更改。

Most commonly, forks are used to either propose changes to someone else's project or to use someone else's project as a starting point for your own idea.

最常见的情况是，叉子可以用来改变别人的项目，或者使用其他人的项目作为自己想法的起点。

##### Propose changes to someone else's 
向其他人的项目提出更改建议


A great example of using forks to propose changes is for bug fixes. Rather than logging an issue for a bug you've found, you can:

使用叉子来提出更改的一个很好的例子就是错误修复。与其为您找到的错误记录问题，您可以：

* Fork the repository.

    分叉存储库。

* Make the fix.

    进行修复。

* Submit a pull request to the project owner.

    向项目所有者提交拉取请求。

If the project owner likes your work, they might pull your fix into the original repository!

如果项目所有者喜欢你的工作，他们可能会将你的修补程序放入原始存储库！

Use someone else's project as a starting point for your own idea.

用别人的项目作为自己想法的起点。

At the heart of open source is the idea that by sharing code, we can make better, more reliable software.

在开源的心脏的理念是通过共享代码，我们可以做出更好，更可靠的软件。


When creating your public repository from a fork of someone's project, make sure to include a license file that determines how you want your project to be shared with others.

从别人项目的分支中创建公共存储库时，请确保包含一个许可证文件，该文件确定您希望项目与其他人共享的方式。

For more information on open source, specifically how to create and grow an open source project, we've created Open Source Guides that will help you foster a healthy open source community by recommending best practices for creating and maintaining repositories for your open source project.

有关开放源代码的更多信息，特别是如何创建和发展开放源代码项目，我们已经创建了开放源代码指南，通过推荐用于为开源项目创建和维护资源库的最佳实践，帮助您培养健康的开源社区。

### Fork an example repository
分叉示例存储库

Forking a repository is a simple two-step process. We've created a repository for you to practice with!

分库是一个简单的两步过程。我们已经创建了一个存储库供您练习使用！

1. On GitHub, navigate to the octocat/Spoon-Knife repository.

    在GitHub上，导航到octocat / Spoon-Knife存储库。

2. In the top-right corner of the page, click Fork.

    在页面的右上角，点击叉子。

That's it! Now, you have a fork of the original octocat/Spoon-Knife repository.

而已！现在，你有一个原始的octocat /勺刀库的叉子。

### Keep your fork synced
保持您的叉同步

You might fork a project in order to propose changes to the upstream, or original, repository. In this case, it's good practice to regularly sync your fork with the upstream repository. To do this, you'll need to use Git on the command line. You can practice setting the upstream repository using the same octocat/Spoon-Knife repository you just forked!

您可能会分支一个项目，以便对上游或原始存储库提出更改建议。在这种情况下，定期将叉与上游存储库同步是一种很好的做法。要做到这一点，你需要在命令行上使用Git。您可以练习使用刚分叉的同一个octocat / Spoon-Knife存储库设置上游存储库！

#### Step 1: Set up Git
第1步：设置Git

If you haven't yet, you should first set up Git. Don't forget to set up authentication to GitHub from Git as well.

如果你还没有，你应该首先设置Git。不要忘记从Git设置身份验证到GitHub。

#### Step 2: Create a local clone of your fork
第2步：创建您的叉的本地克隆

Right now, you have a fork of the Spoon-Knife repository, but you don't have the files in that repository on your computer. Let's create a clone of your fork locally on your computer.

现在，您有一个勺子刀库的分支，但是您的计算机上没有该存储库中的文件。让我们在您的计算机上本地创建一个克隆。

1. On GitHub, navigate to your fork of the Spoon-Knife repository.

在GitHub上，导航到勺子刀库的叉子。

2. Under the repository name, click Clone or download.

在存储库名称下，单击克隆或下载。

3. In the Clone with HTTPs section, click  to copy the clone URL for the repository.

在“克隆与HTTPs”部分中，单击  复制存储库的克隆URL。

4. Open Terminal.

打开终端。

5. Type git clone, and then paste the URL you copied in Step 2. It will look like this, with your GitHub username instead of YOUR-USERNAME:

键入git clone，然后粘贴您在步骤2中复制的URL。它将如下所示，使用您的GitHub用户名代替YOUR-USERNAME：

```
$ git clone https://github.com/YOUR-USERNAME/Spoon-Knife
```

6. Press Enter. Your local clone will be created.

按Enter键。您的本地克隆将被创建。

```
$ git clone https://github.com/YOUR-USERNAME/Spoon-Knife
Cloning into `Spoon-Knife`...
remote: Counting objects: 10, done.
remote: Compressing objects: 100% (8/8), done.
remove: Total 10 (delta 1), reused 10 (delta 1)
Unpacking objects: 100% (10/10), done.
```
Now, you have a local copy of your fork of the Spoon-Knife repository!

现在，您有一份勺子刀叉库的本地副本！

#### Step 3: Configure Git to sync your fork with the original Spoon-Knife repository

第3步：配置Git将您的叉与原始勺子刀库进行同步

When you fork a project in order to propose changes to the original repository, you can configure Git to pull changes from the original, or upstream, repository into the local clone of your fork.

为了向原始存储库建议更改而分叉项目时，可以将Git配置为将更改从原始存储库或上游存储库拖到叉的本地克隆中。

1. On GitHub, navigate to the octocat/Spoon-Knife repository.

在GitHub上，导航到octocat / Spoon-Knife存储库。

2. Under the repository name, click Clone or download.

在存储库名称下，单击克隆或下载。

3. In the Clone with HTTPs section, click  to copy the clone URL for the repository.

在“克隆与HTTPs”部分中，单击  复制存储库的克隆URL。

4. Open Terminal.

打开终端。

5. Change directories to the location of the fork you cloned in Step 2: Create a local clone of your fork.

将目录更改为您在步骤2中克隆的叉的位置：创建叉的本地克隆。



To go to your home directory, type just cd with no other text.

要转到您的主目录，只需输入cd其他文本即可。

To list the files and folders in your current directory, type ls.

要列出当前目录中的文件和文件夹，请键入ls。

To go into one of your listed directories, type cd your_listed_directory.

要进入您列出的目录之一，请键入cd your_listed_directory。

To go up one directory, type cd ...

要走上一个目录，请输入cd ..。

6. Type git remote -v and press Enter. You'll see the current configured remote repository for your fork.

键入git remote -v并按Enter键。你会看到当前为你的fork配置的远程仓库。

```
$ git remote -v
origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
```

7. Type git remote add upstream, and then paste the URL you copied in Step 2 and press Enter. It will look like this:

键入git remote add upstream，然后粘贴在步骤2中复制的URL，然后按Enter键。它看起来像这样：

```
$ git remote add upstream https://github.com/octocat/Spoon-Knife.git
```

8. To verify the new upstream repository you've specified for your fork, type git remote -v again. You should see the URL for your fork as origin, and the URL for the original repository as upstream.

要验证您为叉指定的新上游存储库，请git remote -v再次键入。您应该看到您的分支的URL为origin，以及原始存储库的URL为upstream。

```
$ git remote -v
origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (fetch)
upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (push)
```
Now, you can keep your fork synced with the upstream repository with a few Git commands. For more information, see "Syncing a fork."


现在，您可以使用几个Git命令让您的fork与上游存储库同步。有关更多信息，请参阅“ 同步分支”。

**Next steps**
下一步

The sky's the limit with the changes you can make to a fork, including:

天空是您可以对叉子进行更改的限制，其中包括：

**Creating branches:** *Branches* allow you to build new features or test out ideas without putting your main project at risk.

创建分支机构： 分支机构允许您构建新功能或测试创意，而不会让主项目处于风险之中。

**Opening pull requests:** If you are hoping to contribute back to the original repository, you can send a request to the original author to pull your fork into their repository by submitting a pull request.

打开拉取请求：如果您希望回馈到原始存储库，则可以向原始作者发送请求，以通过提交拉取请求将您的叉拉入其存储库。

### Find another repository to fork
找到另一个存储库来分支

Fork a repository to start contributing to a project. You can fork any public repository, or any private repository you can access. For more information, see "About forks."

分配一个存储库以开始为项目做出贡献。您可以派生任何公共存储库或任何可以访问的私有存储库。有关更多信息，请参阅“ 关于叉子”。

You can browse Explore to find projects and start contributing to open source repositories. For more information, see "Finding open source projects on GitHub."

您可以浏览Explore以查找项目并开始贡献开源库。有关更多信息，请参阅“ 在GitHub上查找开源项目 ”。


### Celebrate
庆祝

You have now forked a repository, practiced cloning your fork, and configured an upstream repository. What do you want to do next?

您现在分叉了一个存储库，练习克隆您的分叉，并配置了一个上游存储库。你想下一步该做什么？

"Set up Git"

“ 设置Git ”

"Create a repository"

“ 创建一个存储库 ”

Fork a repository

分叉储存库

"Be social"

“ 社交 ”

Connect with people around the world in the GitHub Community Forum

在GitHub社区论坛中与世界各地的人联系