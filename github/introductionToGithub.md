# GitHub - Introduction to Git

## Introduction
In order to see full documentation, please <a href="https://learn.microsoft.com/en-gb/training/modules/intro-to-git/?WT.mc_id=cloudskillschallenge_ef5f9f41-0818-4895-9217-79d19827a322">this link</a>.

Git is used to version control code. With Git you can collaborate along with several members of the same team, to make sure that you're using the latest versions of the code for a project, such as <i>terraform modules</i> or <i>html</i> code. For more information, watch this recap of <a href="https://www.youtube.com/watch?v=9uGS1ak_FGg">Introduction to Git Recap</a> offered by Sarah Guthals.

## What is Version Control?
In order to see full documentation, please <a href="https://learn.microsoft.com/en-gb/training/modules/intro-to-git/1-what-is-vc">this link</a>.

A VCS, or <i>Version Control System</i>, is a program or a set of programs that tracks changes to a collection of files. This can be used to recall earlier versions of a file, or an entire project. It is also used so that members of a team can work on the same files, at the same time without affecting each other's work. By leveraging a VCS you can:

* See all the changes that were made to a project, when the changes were made and who made the changes
* Include a message with each change to explain the reasoning behind the change
* Retrieve past versions of the entire project or of individual files
* Create <i>branches</i> where changes can be made experimentally. Once a change has been made, and it is tested and approved, the branch can be <i>merged</i> with the main branch, fusing the changes made in the experimental branch with the branch that is used for production code
* Attach a tag to a version, for example, to mark a new release

### Distributed Version Control
Earlier instances of VCSes used a centralized server for storing the entire project, meaning that a project has a <i>Single Point Of Failure (SPOF)</i>. This changed with Git, as Git is distributed meaning that a project's complete history is stored both the server as well as on the clients. This allows for files to be altered without having network access. File can then be checked in, and once the connection with the server is restored, the changes can be pushed to it.

### Git Terminology
In order to understand Git, it is important to understand the terminology used.

| Term           | Meaning |
| -------------- | --- |
| `Working tree` | The set of nested directories and files that contain the project that's being worked on |
| `Repository/Repo` | The directory, located at the top level of the working tree, where GIt keeps all the history and metadata for a project |
| `Hash` | A number produced by a hash function that represents the contents of a file or another object as a fixed number of digits. Git uses hashes to determine of the contents of a file for example has changed. If the date and time has changed, but the hash hasn't, then Git knows that the content of the file remains the same |
| `Object` | A Git repo contains fpir type of objects, <i>blob</i>, <i>tree</i>, <i>commit</i>, and <i>tag</i>. A Blob contains an ordinary file. A tree object represents a directory (containing names, hashes, and permissions). A Commit object represents a specific version of the working tree. A Tag is a name attached to a commit |
| `Commit` | A commit means that you upload changes so that others can see them (given that you push your changes to the repo) |
| `Branch` | A Branch is a named series of linked commits. Branches allows for several users to work on the same versions of the main-branch at the same time |
| `Remote` | A remote is a named reference to another Git repository. When you create a repo, Git creates a remote named <i>origin</i> that is the default remote for push and pull operations |
| `Commands` | Commands are Git operations performed using commands like "git push" and "git pull" |
