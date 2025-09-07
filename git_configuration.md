# Configure your GitHub account to an AWS instance
## Usecase:
* ### Using your AWS instance (EC2) to push/pull code from GitHub.
* ### using GitHub Actions (CI/CD) to deploy directly to your AWS instance.
#### Steps
1. Install Git on your AWS instance  
		sudo apt update && sudo apt install -y git   # Ubuntu/Debian  
		sudo yum install -y git                      # RHEL/CentOS/Amazon Linux    
2. Configure Git with your GitHub identity  
		git config --global user.name "your-github-username"  
    git config --global user.email "your-email@example.com"  
3. Generate an SSH key on your AWS instance  
		use ssh-keygen   
		cat ~/.ssh/id_ed25519.pub and Copy the output.  
		Go to GitHub → Settings → SSH and GPG keys → New SSH Key.  
		Paste it and save.  
4. Test connection to GitHub  
		ssh -T git@github.com  

##### Example  
If successful, you’ll see:
	
	ubuntu@ip-172-31-27-103:~/.ssh$ ssh -T git@github.com  
	The authenticity of host 'github.com (140.82.113.3)' can't be established.
	ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
	This key is not known by any other names.
	Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
	Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
	Hi kumaramitaryan! You've successfully authenticated, but GitHub does not provide shell access.
	ubuntu@ip-172-31-27-103:~/.ssh$


#### Then set your repo and test 
git remote set-url origin git@github.com:kumaramitaryan/CloudTrainDevopsAI.git

ubuntu@ip-172-31-27-103:~/amit/CloudTrainDevopsAI$ ssh -T git@github.com  
Hi kumaramitaryan! You've successfully authenticated, but GitHub does not provide shell access.  

##### ubuntu@ip-172-31-27-103:~/amit/CloudTrainDevopsAI$ git push origin main
Enumerating objects: 7, done.  
Counting objects: 100% (7/7), done.  
Delta compression using up to 2 threads  
Compressing objects: 100% (6/6), done.  
Writing objects: 100% (6/6), 4.85 KiB | 4.85 MiB/s, done.  
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0  
remote: Resolving deltas: 100% (2/2), done.  
To github.com:kumaramitaryan/CloudTrainDevopsAI.git  
   6a768c0..867abe4  main -> main  
ubuntu@ip-172-31-27-103:~/amit/CloudTrainDevopsAI$  

