AWS Cloudshell is a browser-based, pre-authenticated shell that you can launch direclty from the AWS Management Console
- You can navigate to CloudShell from the AWS Management Console a few different ways
- You can run AWS CLI commands using your preferred shell, such as Bash, Powershell, or Z shell
- You can do this without downloading or installing command line tools

When you launch AWS Cloudshell, a compute environment that's based on AWS Linux 2023 is created.
- Within this environment, you can access:
	- An extensive range of pre-installed development tools
	- Options for uploading and downloading files
	- File storage that persists between sessions
- You can use CloudShell in the most recent versions of Google Chrome, Mozilla Firefox, Microsoft Edge and Apple Safari browsers

#### Features of AWS CloudShell

**AWS Command Line Interface**
- You can launch AWS Cloudshell from the AWS Management Console
- The AWS credentials that you used to sign in to the console are automatically available in a new shell session
- Since AWS users are pre-authenticated, you do not need to configure credentials when interacting with AWS services using [[AWS CLI]] versions 2
- [[AWS CLI]] comes pre-installed on the shell's compute environment

**Shells and Development Tools**
- With the shell that's created for AWS Cloudshell sessions, you can switch seamlessly between your preferred command line shells
- More specifically you can switch between Bash, Powershell, and Z shell
- You also have access to pre-installed tools and utilities
	- Git
	- Make
	- Pip
	- Sudo
	- Tar
	- Tmux
	- Vim
	- Wget
	- Zip
- The shell environment is pre-configured with support for several leading major software languages
	- Node.js
	- Python
	- .NET

**Persistent Storage**
- With AWS CloudShell, you can use up to 1 GB of persistent storage in each AWS Region at no additional cost
- Persistent storage is located in your home directory ($HOME) and is private to you
- Unlike ephemeral environment resources that are recycled after each shell session ends, data in your home directory persists between sessions

**CloudShell VPC Environments**
- AWS CloudShell [[Amazon Virtual Private Cloud (VPC)]] enables you to create a CloudShell environment in your VPC
- For eahc VPC environment, you can assign a VPC, add a subnet, and associate one or more security groups
- AWS Cloudshell inherits the network configuration of the VPC and enables you to use AWS Cloudshell securely within the same subnet as other resources in the VPC

**Security**
- The AWS Cloud Shell environment and its users are protected by specific security features. This includes such features as [[AWS Identity and Access Management (IAM)]] permissions, shell session restrictions, and Safe Pastes for text input
- **Permissions Management with IAM**
	- As admin, you can grant and deny permissions to AWS CloudShell users using IAM policies
	- You can also create policies that specify the particular actions that users can perform with the shell environments
- **Shell Session Management**
	- Inactive and long running sessions are automatically stopped and recycled
- **Safe Paste for Text Input**
	- Safe Paste is enabled by default
	- This security feature requires that you verify that the multiline text that you want to paste into the shell does not contain malicious scripts

**Customization Options**
- You can customize your AWS CloudShell experience to your exact preference
- displayed text sizes, toggle between light and dark mode interfaces themes etc.

**Session Restore**
- The sessions restore functionality restores sessions that you were running across single or multiple browser tabs in the CloudShell terminal
- IF you refresh or reopen recently closed browser tabs, this functionality resumes the session until the shell is stopped because of inactive session
- To continue using your CloudShell session, press any key within the terminal window
- Session restore also restores the latest terminal output and running processes in each terminal tabs

#### Pricing for AWS CloudShell
AWS CloudShell is an AWS service that's available at no additional charge
- However, you pay for other AWS resources that you run with AWS CloudShell
- Moreover, data transfer rates still apply