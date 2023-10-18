# Push your code from the local (PC) directory to the remote (GitHub) repository using Git

## Step 1
`git init`

## Step 2
`git add .`

This command adds all the _**files**_ and _**folders**_ in the local (PC) directory

## Step 3
`git status`

This is optional

## Step 4
`git commit -m "commit message"`

## Step 5
`git remote add origin <GitHub repository link>`

## Step 6
`git push -u origin main`

error: failed to push some refs to '__GitHub repository link__'

### This error occurs due to _branch mismatch_

## Step 7
`git branch`

Output is **master**

Your local branch is called __master__ but the remote branch is called __main__

### These two branches need to be _the same_

## Step 8
`git branch -m master main`

Now both the local and the remote branches are called _**main**_

## Step 9
`git branch`

Output is __main__

### _branch mismatch_ problem has been taken care of

## Step 10
`git push -u origin main`

error: failed to push some refs to '__GitHub repository link__'

hint: Updates were rejected because the remote contains work that you do not have locally

You will get __Updates were rejected__ error even if you have just a single `README.md` file in your __GitHub repository__

### This error occurs due to the already existing works in the _GitHub repository_

## Step 10
`git pull origin main`

Unfortunately the existing works in the **GitHub repository** have not been downloaded in our local directory

__Rather it shows__

fatal: refusing to merge unrelated histories

## Step 11
`git pull origin main --allow-unrelated-histories`

Now, the existing works present in the **GitHub repository** have been downloaded in our local directory

We are ready to push our code to __GitHub__ finally

## Step 12
`git push -u origin main`

Refresh your __GitHub repository__ to see your new work in there

> You actually do need need 12 steps. I explained the process like that to address the errors that occur frequently. You can get the job done in 7 steps only.

>> This is what you actually need to do
- Step 1: `git init`
- Step 2: `git add .`
- Step 3: `git commit -m "commit message"`
- Step 4: `git branch -m master main`
- Step 5: `git remote add origin <GitHub repository link>`
- Step 6: `git pull origin main --allow-unrelated-histories`
- Step 7: `git push -u origin main`

# These 7 steps should be `enough` to get the job done
