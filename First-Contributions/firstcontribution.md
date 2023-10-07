# First Contributions

Contributing to a GitHub repository is a great way to get involved in open-source projects. The [CONTRIBUTING.md](https://github.com/rcallaby/Learn-Git/blob/main/CONTRIBUTING.md) file is often used to provide guidelines for contributors. However, this repository has a [contributors.md](https://github.com/rcallaby/Learn-Git/blob/main/CONTRIBUTORS.md) file specifically for recognizing contributors, you can follow these steps to make your first contribution:

### Fork the Repository

![fork]([First-Contributions/fork.png](https://github.com/RileeyL/Learn-Git/blob/f12392c89debfa0e26fb8018536e00d7a635d5ac/First-Contributions/fork.png))

[Forking](https://docs.github.com/en/get-started/quickstart/fork-a-repo) creates a copy of the repository under your GitHub account.

Go to the repository you want to contribute to. In this case, you want to contribute to this repository.
Click the "Fork" button in the top-right corner of the repository's page.
Wait for GitHub to create a copy of the repository under your account.

### Clone Your Fork

To work on the project locally, you'll need to [clone](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository) your fork to your computer.

On your forked repository page, click the "Code" button, and copy the repository URL (e.g., `https://github.com/[yourusername]/Learn-Git.git`).
Open your terminal or Git bash.
Use the git clone command to clone the repository:
```
git clone https://github.com/[yourusername]/Learn-Git.git

```
### Create a Branch

Before making changes, create a [new branch](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-a-branch-for-an-issue) to work in. This helps keep your contributions organized and separate from the main code.

```
cd repository
git checkout -b your-branch-name

```
Replace your-branch-name with a descriptive name for your branch, such as fix-typo or add-feature.

### Make Your Contribution

Now it's time to make your contribution. This can involve editing code, documentation, or in this case, the [contributors.md](https://github.com/rcallaby/Learn-Git/blob/main/CONTRIBUTORS.md) file. Open the file in your favorite text editor and add your name to the list of contributors following the project's guidelines.

### Commit Your Changes

After making your changes, save the file and commit it to your branch.

```
git add contributors.md
git commit -m "Add [Your Name] to contributors.md"

```
### Push Your Changes

[Push your branch](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/making-changes-in-a-branch/pushing-changes-to-github) with the changes to your GitHub repository.

```
git push origin your-branch-name
```
### Create a Pull Request

Now, go to your forked repository on GitHub. You should see a notification suggesting you create a [pull request](https://docs.github.com/en/pull-requests). Click on it or navigate to the "Pull Requests" tab and create a new [pull request](https://docs.github.com/en/pull-requests).

Ensure that you're comparing your branch with the original repository's main branch. Write a clear and descriptive title and comment explaining your changes. Then, submit the [pull request](https://docs.github.com/en/pull-requests).

### Review and Collaboration

Wait for the project maintainers to review your pull request. They may ask for changes or provide feedback. Be patient and open to suggestions. Continue to make changes and push commits as needed.

### Your Contribution is Merged

Once your contribution is approved, it will be merged into the main repository. Congratulations! You've successfully made your first contribution to a [contributors.md](https://github.com/rcallaby/Learn-Git/blob/main/CONTRIBUTORS.md) file on a GitHub repository.

Remember, each project may have its specific contribution guidelines, so always check the repository's [CONTRIBUTING.md](https://github.com/rcallaby/Learn-Git/blob/main/CONTRIBUTING.md) or other documentation for any project-specific instructions.

Please be kind and give this repository a star ⭐ if you found it to be helpful or useful. Doing so will help others find it and contribute to it.
