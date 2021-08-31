## Practice Git

Here's Everything that you're going to learn in this tutorial:

- Forking and cloning a remote repository via HTTPS.
- Adding the upstream repository to your local development environment.
- Creating and working with branches.
- Understanding project development and contribution work flows.
- Learning to use basic git commands such as: commit, add, push.
- Pushing the changes to your fork and creating a PR to the upstream repository.

That was a mouthful, follow the steps below to practice!

### Forking and Cloning a remote repository

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

### Adding the upstream repository to your local development environment

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

### Creating and working with branches

Branches are, literally just branches to your workflow. You can have multiple
branches for your repository where each branch can have its own name and
possibly, have different code from the main/master branch.
The idea of branches is to move away from the main/master branch and tinker
around and work on new ideas/implementations and use that branch to reference
for raising PRs and `merging` the new changes/implementations to the main/master branch.
Follow these steps on creating a new branch and check-out (A fancy term to say
activate) the same.
To learn more about branches, head over to the [official documentation](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches).

Assuming that you are in the same working directory of the cloned repository.

- Type the following in your command prompt:

```sh
git branch feat-0
```

- Here, `feat-0` is the name of the branch you have just created.
- To see all the branches you have:

```sh
git branch -a
```

- Now, to activate that branch, type the following command:

```sh
git checkout feat-0
```

- You will now be prompted that you have succesfully changed your branch to `feat-0`.

### Understanding project development and contribution work flows
