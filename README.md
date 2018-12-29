# Site Clone
This project serves as an improved instruction manual over my [video](https://www.youtube.com/watch?v=K21WClcKo4g) on how to clone a Website and host it with Firebase Hosting. The instructions in my video are heavily Linux / MacOS operating system focused, whereas these instructions cater to Windows too.


## Differences between the instructions here and the video
- These instructions cater to Windows, Mac, and Linux rather than Linux / MacOS systems alone.
- Here we use a NPM deployment script which is operating system agnositc, rather than a bash script (like in my video).


### Step 1: Install dependencies


#### Windows instructions
1. Open up a command prompt as administrator
<img src="images/cmd-admin.jpg" width="500">
2. Install Chocolatey package manager by entering:

```
@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
```
3. In the same command prompt window, use Chocolatey to install Wget:

```
choco install wget
```
4. [Install Visual Studio Code](https://code.visualstudio.com/download)
5. [Install Node.js (installs NPM at the same time)](https://nodejs.org/en/download/)

#### Mac instructions
1. Open up a terminal.
2. Install Homebrew package manager by entering:

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
3. In the same terminal window, use Homebrew to install Wget:

```
brew install wget
```
4. [Install Visual Studio Code.](https://code.visualstudio.com/download)
5. [Install Node.js (installs NPM at the same time).](https://nodejs.org/en/download/)


#### Ubuntu instructions
1. Open up a terminal.
2. Enter:
```
sudo apt-get install wget
```
3. [Install Visual Studio Code.](https://code.visualstudio.com/download)
4. [Install Node.js (installs NPM at the same time).](https://nodejs.org/en/download/)


### Step 2: Add the NPM deploy script
1. Open up your Firebase project in Visual Studio Code.
2. Open up the integrated command prompt / terminal by pressing `ctrl + backtick` on your keyboard. You can also open this up from the top menu bar by going to `terminal > new terminal`.
3. In the terminal, type `npm init`. You can accept all the default in the interactive prompt, or enter details to suit your project.
4. This should create a file named `package.json`.