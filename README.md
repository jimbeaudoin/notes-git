# notes-git
Git Notes for Myself

Install Latest Version
```sh
sudo add-apt-repository ppa:git-core/ppa
sudo apt-get update
sudo apt-get install git
```
git reset
```sh
--soft  # The staged snapshot and working directory are not altered in any way
--mixed # The staged snapshot is updated to match the specified commit, 
        # but the working directory is not affected. (default)
--hard  # The staged snapshot and the working directory are both updated to match
        # the specified commit
        
```
Unclassified
```sh
# Show Change History for a File
git log -p <filename> 
# Set User Email
git config --global user.email "your_email@example.com"
```

--
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/80x15.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">notes-git</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://jim-beaudoin.com" property="cc:attributionName" rel="cc:attributionURL">Jimmy Beaudoin</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
