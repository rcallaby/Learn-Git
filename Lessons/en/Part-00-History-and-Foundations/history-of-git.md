# History and Foundations of Git

# Introduction

Git is a distributed version control system that was created by Linus Torvalds in 2005. Git represents history in a fundamentally different way than centralized version controls systems (CVCS) such as Team Foundation Version Control, Perforce, or Subversion. Centralized systems store a separate history for each file in a repository. Git stores history as a graph of snapshots of the entire repository. These snapshots, called commits in Git, can have multiple parents, creating a history that looks like a graph instead of a straight line. This difference in history is incredibly important and is the main reason users familiar with CVCS find Git confusing.

Git is important to learn today because it is widely used by developers and companies around the world. It is an essential tool for managing code changes and collaborating with other developers on projects. Git allows developers to work on code independently and then merge their changes together when they are ready.

## Who created Git

Git was originally authored by Linus Torvalds in 2005 for development of the Linux kernel. Since then, other kernel developers have contributed to its initial development. Junio Hamano has been the core maintainer since 2005.

## The Reason Why Git was created

The original team could no longer use BitKeeper, a previous version control system, after losing their free license to use it. At the time, no other Source Control Management (SCMs) met their specific requirements for a distributed system. Some of the goals of the new system were speed, simple design, strong support for non-linear development (thousands of parallel branches), fully distributed and able to handle large projects like the Linux kernel efficiently (speed and data size).

## Alternatives to Git

There are several alternatives to Git, including Subversion (SVN), Mercurial (Hg), and Perforce.

Subversion is a centralized version control system that is similar to CVS. It is often used in enterprise environments because it is easy to use and has good integration with other tools.

Mercurial is a distributed version control system that is similar to Git. It is often used in smaller projects because it is easier to learn than Git.

Perforce is a centralized version control system that is often used in enterprise environments. It has good support for large files and binary files.

Each of these systems has its own strengths and weaknesses, and the choice of which one to use depends on the specific needs of the project. Git is widely used by developers and companies around the world because it is an essential tool for managing code changes and collaborating with other developers on projects. Git allows developers to work on code independently and then merge their changes together when they are ready.

## Where to store your repositories for free

There are several free places on the Internet where you can store your Git repositories. Here are some of the most popular ones:

- GitHub
- GitLab
- Bitbucket
- SourceForge

Each of these services has its own strengths and weaknesses, and the choice of which one to use depends on the specific needs of the project. GitHub is the most popular service and is widely used by developers and companies around the world. It offers unlimited public repositories and a limited number of private repositories for free. 

GitLab is another popular service that offers unlimited private repositories for free. Bitbucket is a service that is often used by small teams because it offers unlimited private repositories for free for up to five users. SourceForge is a service that has been around for a long time and is often used for open source projects.