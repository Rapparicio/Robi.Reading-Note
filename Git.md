# Git stores data by taking snapshots of the information.


[Git Tutorial](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/#1###Snapshots)

Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. 
If the file has not changed, Git only stores a reference to the already-stored identical version of it.

- Local Operations

Git mostly relies on local operations because most necessary information can be found in local resources. 
This allows for process expediency because a project’s history resides on the local disk, eliminating the need to fetch history information from the server, and allowing one to continue work on a project even when not online or on a VPN.

- Tracking Changes

Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.

- Loss of Data

Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. 
Git makes it extremely difficult for a snapshot of your file that is committed to be lost.

- States

Files in Git can reside in three main states: committed, modified and staged.

- Committed

Data is securely stored in a local database

- Modified

File has been changed but not committed to the database

![image](https://user-images.githubusercontent.com/73135321/126853874-8d639f21-83a7-42fb-bff0-43ba67ca0260.png)

### The Life Cycle of File Status
After you edit a file, Git flags it as modified because of changes made after the previous commit.
You stage the modified file.
Then, you commit staged changes.
![image](https://user-images.githubusercontent.com/73135321/126853918-84a5cc63-c0c0-4b03-b8b3-abedd405fc73.png)

## Remote Repositories
In order to collaborate on Git projects, you must interact with remote repositories, versions of a project residing online or on a network. You can work with multiple repositories, for which you can have read/write or read-only privileges. Teams can use remote repositories to push information to and pull data from.

Cloned Repositories
As mentioned earlier, for cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local branch.

Seeing Your Remotes
By running the git remote command, you can view the short names, such as “origin,” of all specified remote handles.

By using git remote -v, you can view all the remote URLs next to their corresponding short names.
