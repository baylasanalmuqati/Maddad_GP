## Push a folder to GitHub from the command line

Use this quick guide to upload an existing local folder to a GitHub repository with Git. Make sure Git is installed, you have a GitHub account, and you know the repository URL.

1. Open a terminal in the folder you want to push.
2. Initialize Git (skip if the folder is already a repo):
   ```bash
   git init
   ```
3. Add all files and commit:
   ```bash
   git add .
   git commit -m "Initial commit"
   ```
4. Set the remote to your GitHub repo (replace the URL with yours):
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   ```
5. Push to the main branch (create it if needed):
   ```bash
   git branch -M main
   git push -u origin main
   ```

If you cloned an existing repository instead, skip steps 2–4 and just run `git add .`, `git commit -m "<message>"`, and `git push`.
