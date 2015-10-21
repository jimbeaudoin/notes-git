# notes-git
Git Notes for Myself

### Install Latest Version
```sh
sudo add-apt-repository ppa:git-core/ppa
sudo apt-get update
sudo apt-get install git
```
### Init Setup
```sh
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```
### Default Editor
```sh
git config --global core.editor vim
```

### git reset
```sh
--soft  # The staged snapshot and working directory are not altered in any way
--mixed # The staged snapshot is updated to match the specified commit, 
        # but the working directory is not affected. (default)
--hard  # The staged snapshot and the working directory are both updated to match
        # the specified commit
```

### Create Bare Directory
```sh
mkdir <project_name>.git
cd <project_name>.git
git init --bare
```

### Private Remote Server
```sh
# 1. Create a Bare Repository on the Remote Server
# 2. Add the Remote Server to the local Git Repository
# 3. Git Push

git remote add <remote_name> <ssh_info>:<bare_git_repos_path>
```

### Development commands
```sh
# Rebase & squash
git rebase -i HEAD~5
# Rename a branch
git branch -m <old_name> <new_name>
```

### Unclassified
```sh
# Show Change History for a File
git log -p <filename>
git ls-files | xargs wc -l # Show how many lines of code per files and total
```

--
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/80x15.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">notes-git</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://jim-beaudoin.com" property="cc:attributionName" rel="cc:attributionURL">Jimmy Beaudoin</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
