# Step-By-Step Procedure of Setting Up Git,Github, and VSC (Visual Studio Code)
So you want to start coding? Well, there are many tools around the internet you can use to start coding, but these three components will help you jumpstart your journey with coding. I am Angelo of BSCpE 1-1, and today I will help you install Git, Visual Studio Code (VSC) and setup your own account at Github.
#### Ready to Start?
#### Alright! Let's go first with installing Git!
## Installing Git
Git is a free, open-source tool for tracking changes to files, especially code, over time. Think of it as a "time machine" or advanced "undo" button for your projects. It lets you save snapshots of your work, go back to older versions, and collaborate without losing anything. So how do you install it into your device?

1. Open your web browser and search Git download or go to this link https://git-scm.com/

![Git Website](/Pictures/Git%20Website.png)

2.	Go to install

![Install Git](/Pictures/Install%20Git.png)

3.	Select which OS (Operating Software) you are currently using, and follow the corresponding instructions how to download it (In this case, select the "Git for Windows/x64 Setup." for windows in the "Standalone Installer" row).

![Git Installer Web](/Pictures/Git%20Installer%20Web.png)

4.	After it has been downloaded, click the installer in your downloads folder.

![Git Installer](/Pictures/Git%20Installer.png)

5.	Follow the instructions and click next.

![Git Finish Installing](/Pictures/Git%20Finish%20Installing.png)

6.	After the installation, there are two ways to check if Git has been installed in your computer:
*	First Way : Go to a folder in your computer and press right click inside of it, then go to "Show More Options" and if you see a "Git Bash" and "Git GUI" then git has been installed into your computer. (If you are using Windows 10, just right click your mouse into the empty folder and you can already see if Git is installed in your computer)

![Git Bash in Folder](/Pictures/Git%20Bash%20In%20Folder.png)

*   Second Way : Go to your computer's search bar and search Git and it will pop up if your Git isn't installed.

![Git Bash in Search Bar](/Pictures/Git%20Bash%20in%20Search%20Bar.png)

## Setting Up GitHub
GitHub is like this giant online storage locker and collaboration hub for people who build software, write code, or manage projects. It's built on a tool called Git, which helps track changes to files over time, kind of like a "save" button with a history log. Think of it as Google Drive for programmers, but with extra features for teamwork and sharing.
1.	Open your web browser and search GitHub or go to this link https://github.com/

![GitHub Website](/Pictures/GitHub%20Website.png)

2.	Go to Sign up that is located at the upper right of the website.

![GitHub Sign Up](/Pictures/GitHub%20Sign%20Up.png)

3.	Create your account follow the procedures displayed on the process.
4.	That's it, you're done setting up your GitHub account!

We will go back on how GitHub is used, but for now let's go on how-
## How to Download Visual Studio Code (VSC)
1.	Open your web browser and search Visual studio code or go to this link https://code.visualstudio.com/

![VSC Website](/Pictures/VSC%20Website.png)

2.	Click Download located at the top right of the website.

![Download VSC](/Pictures/Download%20VSC.png)

3.	It will take you to the download page and will show you the different installers for different operating systems.

![VSC Installer](/Pictures/VSC%20Installer.png)

4.	Click the operating software you are using and the file will be downloaded to your computer.
5.	After that, click the installer located at your computer's download folder and follow the steps necessary in the installer.

![VSCODE Installer](/Pictures/VSCODE%20Installer.png)

6.	And you're done! To check if VSC has been successfully downloaded, go to your computer's search bar and search the Visual Studio Code to see if the software is in your computer.

![VSC Installing Finish](/Pictures/VSC%20Installing%20Finish.png)

![VSC In Search Bar](/Pictures/VSC%20in%20Search%20Bar.png)

## Congratulations! You have now the essential parts in starting your journey to coding!

Now, after installing both GitHub and Git, here's how you can start a repository and directly link your code through Visual Studio Code

## Starting A Repository
A repository (often called a "repo") is a central storage location for managing, tracking, and collaborating on files and code. In the context of version control systems like Git, it's a folder that contains all the files for a project, along with the history of changes made to them.

So, how do you start one?

1.	Log In to GitHub:
Go to github.com and sign in.

2. Create a New Repository:
Click the "+" icon in the top-right corner (next to your profile picture).
Select "New repository" from the dropdown.
![GitHub New Repository](/Pictures/GitHub%20New%20Repository%20.png)

3. Configure the Repository:

 - **Repository Name**: Enter a unique name (e.g., "my-project").

 - **Description**: Add an optional short description.

 - **Visibility**: Choose "Public" (free and visible to everyone) or "Private" (requires a paid plan for private repos).

    Leave "Initialize this repository with" unchecked if you want to start empty.

![GitHub Repository Details](/Pictures/GitHub%20Repository%20Details.png)


4. Create the Repository:
Click "Create repository". GitHub will generate the repo and show its URL (e.g., https://github.com/yourusername/my-project.git).

![New Repository](/Pictures/New%20Repository.png)

## Linking VS Code to GitHub 
1.	Open VS Code and Access the Terminal:
    - Launch VS Code.
    - Open the integrated terminal: View > Terminal (or Ctrl+ / Cmd+ on Mac).

2. Run the Provided Git Configuration Commands:
    - In the terminal, execute each command one by one (replace placeholders with your details):
        * git config --global user.name "Your Name"
        * git config --global user.email "you@youraddress.com"
        * git config --global push.default matching
        * git config --global alias.co checkout
    - These set up your Git identity and preferences globally (across all repos on your machine).

3.	Initialize a Local Repository (If Starting a New Project):
    - Navigate to your project folder in the terminal (e.g., cd path/to/your/project)
    - Run: git init
    - This creates a .git folder, turning the directory into a Git repo. You can now add files and commit them.

4. Authenticate with GitHub:
    - VS Code can handle this via its UI. Click the Accounts icon (person silhouette) in the bottom-left, then "Sign in with GitHub" to authorize via OAuth (opens a browser).
    - Alternatively, for command-line pushes, set up a Personal Access Token (PAT) on GitHub (Settings > Developer settings > Personal access tokens) and use it as your password when prompted.

5. Connect to an Existing GitHub Repository:
    - Clone a Repo: In VS Code, open the Command Palette (Ctrl+Shift+P / Cmd+Shift+P), type "Git: Clone", paste the GitHub URL (e.g., https://github.com/username/repo.git), and select a folder. VS Code will clone it and open it.
        * git remote add origin https://github.com/username/repo.git
        * git add .
        * git commit -m "Initial commit"
        * git push -u origin main

6. Verify and Use in VS Code:
    - Open the Source Control view (Ctrl+Shift+G / Cmd+Shift+G) to see changes, commits, and branches.
    - Use the UI for staging, committing, pushing, and pulling. The co alias you set can be used in the terminal (e.g., git co branch-name).
    