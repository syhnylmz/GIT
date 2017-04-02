### PART 1
Source : https://www.youtube.com/watch?v=mYjZtU1-u9Y&list=PL1F56EA413018EEE1
## Start Config
User Name
git config --global user.name <user.name>
git config --global user.name "Seyhan YILMAZ"

User Email
git config --global user.email <email>
git config --global user.email "iletisim@seyhanyilmaz.net"

## Proxy
http://stackoverflow.com/questions/783811/getting-git-to-work-with-a-proxy-server

git config --global http.proxy http://proxyuser:proxypwd@proxy.server.com:8080

change proxyuser to your proxy user
change proxypwd to your proxy password
change proxy.server.com to the URL of your proxy server
change 8080 to the proxy port configured on your proxy server
If you decide at any time to reset this proxy and work without proxy:

Command to use:

git config --global --unset http.proxy

Finally, to check the currently set proxy:
git config --global --get http.proxy


## Starting Git
- Create Git Project
git init <project folder>
git init gitproject

- Check Status
git status

git add. 

git status

git rm --cached <filename>
git rm --cached test.txt

git status

git commit -m "your message"
git commit -m "Initial Commit"
git commit -m "Project Initialiazed"

git log

git status

git add test.txt

git commit -m "start traccking test.txt"

git log

modify readme.txt

git status

git commit -m "change readme"
show error

git add .
git commit -m "change readme"
git log

modify readme.txt
modify test.txt
git add .
git commit -"another commit"

add new file
change readme.txt
git status
git diff
show changed
git add readme.txt
git diff
show nothing
git diff --cached
git status
git add .
git status
git commit -m "new file and changes"

##Shortcuts
git log
when "git log" is too log
shift+zz

git log --oneline

change file
git status
git commit -a -m "short cut"
git log --oneline

git status -s


Step 1 : git init <project>			-> project now repository
Step 2 : git add .					-> add all files to staging
Step 3 : git commit -m "message"	-> snapshot

git status							-> stasus of files
git log								-> commit history
git diff							-> view diffrence
git dif --cached					-> difference in staging


### PART 2
1. Create SSH key					-> We will be using RSA public/private cryptography
2. HTTPS or SSH or SSH either will work GitHub prefers SSH

gitbash
ssh-keygen -t rsa -C "email address"

tets
ssh -T git@github.com

git remote add origin git@github.com:syhnylmz/GIT.git
git remote add origin https://github.com/syhnylmz/GIT.git

git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/syhnylmz/GIT.git
git push -u origin master

remove remote
git remote -v
git remote remove origin
