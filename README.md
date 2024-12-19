1. **Create a project folder & initialize Git**
mkdir project-folder
cd project-folder
git init

2. **Make changes to the project (add files and contents)**
echo "<html>Project content</html>" > index.html

3. **Rename your main branch from 'master' to 'main'**
git branch -m master main

4. **Stage your changes and commit them**
git add .
git commit -m "Initial commit with project content"

5. **Create a GitHub repo and connect it with your project**
git remote add origin https://github.com/Rosine22/git-repo-theGym.git

6. **Push your changes to GitHub**
git push -u origin main

7. **Create a new branch 'dev'**
git checkout -b dev

8. **From 'dev' create another branch 'test'**
git checkout -b test

9. **Go back to the 'dev' branch and delete the 'test' branch**
git checkout dev
git branch -d test

10. **Create a new 'home.html' file, add some HTML changes, and save them**
echo "<html>Home Page</html>" > home.html

11. **Stash save your current changes**
git add home.html
git stash

12. **Repeat the same process for a new 'about.html' page and stash save your changes**
echo "<html>About Page</html>" > about.html
git add about.html
git stash

13. **Repeat the same process for a new 'team.html' page and stash save your changes**
echo "<html>Team Page</html>" > team.html
git add team.html
git stash

14. **Using stash pop, restore the changes of the 'about.html' page**
git stash list
git stash pop stash@{1}

15. **With the help of an index, use stash p
