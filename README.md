## Practice Git

Here's Everything that you're going to learn in this tutorial:

- Forking and cloning a remote repository via HTTPS.
- Adding the upstream repository to your local development environment.
- Creating and working with branches.
- Understanding project development and contribution work flows.
- Learning to use basic git commands such as: commit, add, push.
- Pushing the changes to your fork and creating a PR to the upstream repository.

That was a mouthful, follow the steps below to practice!

#### Forking and Cloning a remote repository

Before you start working with GitHub, you need to have an account. [Sign up](https://github.com/join) for GitHub and come back here.
Now, go to this link and follow these steps to install Git in your computer:
[Click Here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

If you are using Linux, you could use your package manager to install git directly.

To check if you are done installing Git in your local computer, type the following in your command prompt/terminal:

```sh
git --version
```

If you did everything correctly, you will be prompted with the version of Git
your are running. If not, click the link mentioned above and install it correctly.

After you are done with Installing Git, you need to clone this repository.
For that, follow these steps:

- Click on the green Code button you see and you will get a drop down and copy the specified link.
- Now, open up your command prompt/terminal and execute the following:

```sh
git clone https://github.com/hemanth-kotagiri/practice-git.git
```

- The repository is now cloned in your [current working directory](https://www.computerhope.com/jargon/c/currentd.htm).

With this, you now have a local copy of the repository.

#### Adding the upstream repository to your local development environment

It is essential to add the upstream(a fancy way to refer to the original repository that you have cloned) to your local copy.
To do this, follow these steps:

- Make sure that you are in the directory of the cloned repository.
- Type the following command:

```sh
git remote add upstream https://github.com/hemanth-kotagiri/practice-git.git
```

- Now, the upstream repository will be added to your local development environment.
- To check the available remote(s) you have, type the following:

```sh
git remote -v
```

- You will get the following as the output:

```
origin	https://github.com/{YOUR-GITHUB-ID}/practice-git.git (fetch)
origin	https://github.com/{YOUR-GITHUB-ID}/practice-git.git (push)
upstream	https://github.com/hemanth-kotagiri/practice-git.git (fetch)
upstream	https://github.com/hemanth-kotagiri/practice-git.git (push)
```

You are now ready to go for the next step, that is to creating a new branch.
