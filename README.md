# gh-bb-shared-repository

# How to:


From Scratch you can: 

    1. Create an empty repository on both, try to use the same repository name to be eisier to identify
    2. Do the following code:
    ```
        cd path/to/repository
        git init
        # Create a new README.md File
        git add README.md
        git commit -m "First Commit"
        # This will rename the branch name to main
        git branch -M main
        # Ok, in my case, GH will be the pull and push repository so I'll add it first
        git remote add origin git@github.com:rhattox/gh-bb-shared-repository.git
        # After, to add bitbucket you can run this command 
        git remote set-url --add origin git@bitbucket.org:rhattox/gh-bb-shared-repository.gi
        # Double check its remotes
        git remote -v show
        # Push to both repositories
        git push origin main
    ```


for more info, check this link: https://blog.kevinlee.io/blog/2013/03/11/git-push-to-pull-from-both-github-and-bitbucket/