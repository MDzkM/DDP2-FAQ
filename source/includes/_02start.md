# Installation

## Recipes

In this course, you will need to install some applications. There also some additional tools which could come in handy later on. To minimize conflicts, here are the versions of the tools which we will use in this course:

| Application                        | Status           | Recommended Version        |
| ---------------------------------- | ---------------- | -------------------------- |
| An operating system of your choice | Mandatory (duh?) | Please use 64-bit versions |
| Java Development Kit (JDK)         | Mandatory (duh?) | Latest (\>= 10.0)          |
| Git                                | Mandatory        | Latest (\>= 2.26)          |
| Visual Studio Code                 | Recommended      | Latest                     |
| VSCode Java Extension Pack         | Recommended      | Latest                     |
| VSCode Live Share Extension Pack   | Optional         | Latest                     |



## Java

A Java Development Kit (JDK) installation comes with essential things to develop a Java program. Do note that JDK does not come with an editor like Python with its' IDLE. You will need to write your program in a separate editor.

To get the latest version of JDK, go to Oracle's site ([https://www.oracle.com/java/technologies/javase-downloads.html](https://www.oracle.com/java/technologies/javase-downloads.html)), pick your desired JDK version (latest is better), then choose the correct file for each OS, which is:

- Windows x64 Installer for Windows users
- macOS Installer for macOS users
- Linux Compressed Archive for Linux users (If you use Debian-based distros, it is easier to use Linux Debian Package)

### Installation for Windows

- Run the installer which you have downloaded previously (make sure you have administrator access or you are the only user). You don't have to change anything during installation.

   ![image-20200913083855321](../images/java-win-01.jpg)

- After a successful installation, search for "PATH". In Windows 7, 8, and 8.1, the search bar is inside the Start menu/screen. In Windows 10, it is in the taskbar. Choose the recommended result ("Edit the system environment variables").

   ![image-20200913084634050](../images/java-win-02.jpg)

- Choose "Environment Variables" in the settings window. Then, select "Path" in System Variables. Click "Edit" to modify it.

   ![image-20200913084956739](../images/java-win-03.jpg)


- Add your Java installation to the Path entry by clicking "New", then typing Java's default installation folder, and clicking "OK".

  > The JDK 14 directory for Windows is (change 14.0.2 to your JDK version if you install a different one):

  ~~~powershell
  "C:\Program Files\Java\jdk-14.0.2\bin"
  ~~~

  ![image-20200913090129269](../images/java-win-04.jpg)

- Verify that your Java installation is detected by launching a Command Prompt / PowerShell / similar applications.

   > You can use this command to check your JDK version.

   ~~~powershell
   java -version
   ~~~

   ![image-20200913090340871](../images/java-win-05.jpg)



### Installation for macOS

Installation for macOS is usually straightforward. Just run the downloaded file (be sure to give the installer necessary privileges) and the installation should run without any modified settings. To check if the JDK is installed, run <code>java -version</code> in your Terminal.

![Screen Shot 2020-09-13 at 10.07.29](../images/java-mac-01.jpg)

![Screen Shot 2020-09-13 at 10.08.24](../images/java-mac-02.jpg)



### Installation on Linux (.tar.gz)

This installation uses the compressed archive method, which is adaptable to almost all Linux distributions. It is done almost fully in the command line and is tested to work with Bash and Zsh shells by the author of this site.

> Command to extract the archive:

~~~shell
tar xzf jdk-14.0.2_linux-x64.bin.tar.gz
~~~

- First, navigate to the directory where you have downloaded JDK and extract the archive (substitute the file with your version if different).

> Command to move the folder:

~~~shell
mv jdk-14.0.2 $HOME
~~~

- There should be a new folder called "jdk-\<version\>". Now, move that folder to your home directory (you can use $HOME or ~ as an alias for home directory).

> Navigate to home directory:

~~~shell
cd $HOME
~~~

- Now, navigate to your home directory

> Command to add JDK to Path:

~~~shell
echo "export PATH=$(pwd)/jdk-14.0.2/bin:$PATH" >> .bashrc
~~~

- Run the command in the sidebar to add JDK to your Path variable (replace .bashrc with .zshrc if using Zsh)

> Command to reload shell:

~~~shell
source .bashrc
~~~

- Restart your Terminal or run the reload command for the changes to take effect (replace .bashrc with .zshrc if using Zsh)

> Check Java:

~~~shell
java -version
~~~

- To check if JDK is working, run the java command.


![](../images/java-linux-01.jpg)



## Git

Git is a version control system (VCS) designed to help you maintain file versions for projects small and large. In this course, you will get and submit assignment through this application. First of all, we should know the difference between "Git" and "GitHub/GitLab":

| Git                                                   | GitHub/GitLab                                                |
| ----------------------------------------------------- | ------------------------------------------------------------ |
| The software that we can use to manage file versions. | The platform in which we can store files using Git software in the cloud. |



### Installation

> To check whether Git is installed or not, execute the following command:

~~~shell
git --version
~~~

Linux users should have Git bundled with their operating system. On the other hand, Windows and macOS users should download it from Git's website (https://git-scm.com/downloads). Install Git as you would with other applications, but Windows users should pay attention to this menu:

![](https://www.woodwardweb.com/Windows-Live-Writer/Setting-up-the-perfect-Git-environment-o_906F/image_4.png)

In order to use Git using your standard Command Prompt, choose the "Run Git from the Windows Command Prompt" (photo by Martin Woodward).



### Configuration

Before you can start using Git, you must let Git know who you are. To do this, open your Terminal / Command Prompt / similar applications, then use the git config command.

> To fill in user details, execute the following commands:

~~~shell
git config --global user.name "<Your Name Here>"
git config --global user.email "<Your Email Here>"
~~~

This configuration will reflect throughout your system. Later on, you can override this configuration for individual projects.

Also, you may need to tweak the autocrlf feature in Git to avoid collaboration difficulties later on:

> To modify the setting of autocrlf, execute the following command:

~~~shell
git config --global core.autocrlf input
~~~



## Visual Studio Code

Visual Studio Code is a text editor from Microsoft which you can use to write Java programs. It can be extended with some addons to make it a quite powerful development tool.

To install Visual Studio Code on Windows or macOS, download the appropriate installer from the official website ([https://code.visualstudio.com/](https://code.visualstudio.com/)). Install it as you would for other applications.

Linux users are recommended to check with their OS's application manager. For example, Snap Store already has distributions for Visual Studio Code and it is easier to install from there. If such distributions do not exist, you can download it from the official website.

### Java Extension Pack

To aid in Java program development, Microsoft provides a Java Extension Pack which consists of 6 (six) extensions for things such as autocompletion, debugger, syntax checker, etc. More information about this extension can be found in [https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack).

To install this extension from within Visual Studio Code, click the Extension icon (marked in the picture), then type "Java Extension Pack" in the search bar. Select the version published by Microsoft then click Install.

![image-20200913113305929](../images/vsc-01.jpg)



### Live Share Extension Pack

Desperate times call for desperate measure, they said. Since we are now facing a work-from-home scenario, it can be difficult to share code in real-time to be discussed. To support this, Visual Studio Code has an extension called "Live Share Extension Pack" to share your Visual Studio Code contents to others in real-time.

To install this extension, follow the same steps as in installing Java Extension Pack.

![image-20200913114048002](../images/vsc-02.jpg)

For more information on how to use the extension, please refer to [this module](https://docs.google.com/document/d/1wvDzgmEHUUSbzTqz3hsEapj7UZVjUi6TxArhn5K-Dus/edit?usp=sharing).