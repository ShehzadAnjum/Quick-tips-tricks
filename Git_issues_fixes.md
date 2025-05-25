## Git both push and pull fails
- git push is failing because your local main is behind the remote main.
- git pull is failing because your local and remote repositories have unrelated histories.

## 🔧 Root Cause:
You likely created the local repo separately (e.g., with git init) and then tried to connect it to an existing GitHub repo that already had a README or some other commits.

### If you don't need your local commits, and just want to overwrite local with remote, do:
`git fetch origin
git reset --hard origin/main`  
Then your local copy will exactly match the GitHub version.

### 🛠️ Recommended Fix (Merge both histories):
If you want to preserve your local work and merge both:
`git pull origin main --allow-unrelated-histories`
This will fetch and merge the remote branch even though the histories are unrelated.  

Then resolve any merge conflicts (if any), and finally:  
`git push origin main`
