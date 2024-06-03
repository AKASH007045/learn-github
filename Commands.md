# git Commands

git help > // will open editor in terminal for linux and mac , while for windows will open the help page in browser.
        `git help config`

### Git Configuration
git config --global user.name "Akash Sharma"
git config --global user.email "akash007XX@gmail.com"
git config --global --list
git config --global --edit // toedit the global config
git commit --amend --reset-author // to amend the config for previous commits
git config --global init.defaultBranch main //change default branch name on repo initialisation

git branch -m "repo name" // rename a branch to something new
git remote -v // list git remote repositories, with -v verbose it will display the full url

// git will store the global config settings in "~/.gitconfig" file in users home directory.
// minimum required configuration in order to start using Git? Name and Email

## Starting fresh
git init reponame
        git init learngit //it will initialise a new git repository by the name learngit. Which will have a new folder name .git >> which contains files
                HEAD (f)
                config (f)
                description (f)
                hooks (d)
                info (d)
                objects (d)
                refs (d)

## Gitting Historical
git log
        git log --oneline --graph --decorate --color

## Deleting and moving a file
git rm <filename> // it will move to staged area , we will still have to run git commit in order to have it deleted from git.
rm <filename> // this is alternate way by which we can directly delete file without using git, but here we will have to run git add along with git commit.

git mv <filename> <newpath> // it will move to staged area , we will still have to run git commit in order to have it deleted from git.
mv <filename> <newpath>  // this is alternate way by which we can directly move file without using git, but here we will have to run git add along with git commit.

## Ignoring Files
use ".gitignore" // example data : *.log or abc.yaml