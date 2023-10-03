# Learn-Git
This is where you will find a sample repository for my YouTube tutorial series on Learning Git and Github.
If you found this repository to be helpful, please consider giving it a star ⭐ as it will be easier for others to find it.

## Here is a step-by-step tutorial on how to contribute to GitHub
Create a GitHub account: If you don't already have a GitHub account, you'll need to create one. Go to github.com and click the "Sign up" button in the upper right corner. Follow the instructions to create your account.

Find a repository to contribute to: Once you have a GitHub account, you can search for repositories that you're interested in contributing to. You can use the GitHub search bar to search for repositories by name or keyword.

Fork the repository: Once you've found a repository that you want to contribute to, you'll need to fork it. Forking creates a copy of the repository in your own GitHub account, which you can modify without affecting the original repository. To fork a repository, go to the repository's main page and click the "Fork" button in the upper right corner.

Clone the forked repository: After forking the repository, you'll need to clone it to your local machine. Cloning creates a copy of the repository on your computer that you can work on. To clone the repository, open a terminal window and enter the following command:

```
git clone https://github.com/your-username/repository-name.git
```
Be sure to replace "your-username" and "repository-name" with your GitHub username and the name of the repository you forked.

Make sure you create a uniquely named branch to reflect the changes you wish to make to the source code. You can use the following syntax:

```
git checkout -b "branch-name"
```

Make changes to the code: Once you have the repository cloned to your local machine, you can make changes to the code. Use your preferred text editor or IDE to modify the files.

Commit the changes: After making changes to the code, you'll need to commit them to your local repository. To do this, open a terminal window and navigate to the root of the cloned repository. Use the following command to stage the changes:

```
git add .
```
This will stage all changes made to the files in the repository.

Next, commit the changes using the following command:

```
git commit -m "A brief description of the changes made"
```
Be sure to include a brief, informative message describing the changes you made.

Push the changes to GitHub: After committing the changes to your local repository, you'll need to push them to GitHub. This will update the copy of the repository in your GitHub account with the changes you made. To push the changes, use the following command:

```
git push origin branch-name

```
Be sure to replace "branch-name" with the name of the branch you want to push your changes to.

Create a pull request: After pushing the changes to GitHub, you'll need to create a pull request. A pull request is a request for the repository owner to pull in the changes you made and merge them with the original repository. To create a pull request, go to the repository page in your GitHub account and click on the "New pull request" button.

This will take you to a page where you can review your changes and provide a description of your pull request.

Make sure to include a clear and concise description of the changes you made and why you made them.

If there are any issues or concerns that the repository owner should be aware of, make sure to mention them in the pull request description.

Once you're satisfied with the description, click on the "Create pull request" button.

Wait for feedback: After creating the pull request, the repository owner will review your changes and provide feedback.

They may ask you to make additional changes, or they may merge your changes into the original repository.

Be patient and responsive during this process, and make sure to address any feedback or concerns that the repository owner raises.

Update your forked repository: If the repository owner merges your changes into the original repository, you'll need to update your forked repository to reflect those changes.

To do this, navigate to your forked repository on GitHub and click on the "Fetch upstream" button.

Then, run the following command in your local repository to update it:

```
git pull
```

That should give you a brief idea of how to use Git, of course, you can look at the lessons that I have created in this repository for more in-depth explanations.

## Good first issue

You can use this project as a way to start contributing to open-source projects. This could be a **good first issue** just modify the [CONTRIBUTORS.md](https://github.com/rcallaby/Learn-Git/blob/main/CONTRIBUTORS.md) file so that it links to your own GitHub repository. Use markdown as shown in the file. 

Please look at the [First-Contributions](https://github.com/rcallaby/Learn-Git/tree/main/First-Contributions) directory for step-by-step directions on how to contribute to this repository.

### Table of Contents

- [Part 00 - History and Foundation](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-00-History-and-Foundations/history-of-git.md)
- [Part 01 - Basic Navigation](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-01-Basic-Navigation/basic-navigation.md)
- [Part 02 - Initializing Git](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-02-Initializing-Git/getting-started.md)
- [Part 03 - Branching and Merging](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-03-Branching-and-Merging/branching-and-merging.md)
- [Part 04 - Collaborating with Remote Repositories](https://github.com/rcallaby/Learn-Git/tree/main/Lessons/Part-04-Collaborating-with-Remote-Repositories/collaborating-with-remote-repos.md)
- [Part 05 - Advanced Git Concepts](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-05-Advanced-Git-Concepts/advanced-git.md)
- [Part 06 - CI-CD with Git and Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-06-CI-CD-with-Git-and-Github/ci-cd-git-github.md)
- [Part 07 - Git Best Practices and Tips](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-07-Git-Best-Practices-and-Tips/best-practices-tips.md)
- [Part 08 - Git and GitHub in Agile Development](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-08-Git-and-Github-in-Agile-Development/git-github-agile-dev.md)
- [Part 09 - Github and Codespaces](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-09-Github-and-Codespaces/github-codespaces.md)
- [Part 10 - Github Actions](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-10-Github-Actions/github-actions.md)
- [Part 11 - Advanced Github Actions](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-11-Advanced-Github-Actions/advanced-github-actions.md)
- [Part 12 - Using Jupyter Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-12-Using-Jupyter-Codespaces-in-Github/github-jupyter-codespace.md)
- [Part 13 - Using C# Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-13-Using%20C%23-Codespaces-in-Github/github-Csharp-codespace.md)
- [Part 14 - Using React Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-14-Using-React-Codespaces-in-Github/github-react-codespace.md)
- [Part 15 - Using Express Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-15-Using-Express-Codespaces-in-Github/github-express-codespace.md)
- [Part 16 - Using Ruby on Rails Codespaces](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-16-Using-Ruby-on-Rails-Codespaces/github-rubyrails-codespace.md)
- [Part 17 - Using Django Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/Part-17-Using-Django-Codespaces-in-Github/github-django-codespace.md)
