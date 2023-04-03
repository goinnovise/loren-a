# Resume Online Application

## About

This is a jekyll application. Install Jekyll following the instructions for your operation system then execute `jekyll serve` to run the app.

## Update Resume

- To update information, update data.yml
- Information in data.yml maps to pages within the Jykll Application
- Changes committed to `master` branch get auto-deployed to gitbub.io

## To create a resume for a new employee

1. Create a new repo in github: https://github.com/new. Name the repo the employee's name.
2. On your machine navigate to `dev/innovise/resumes` then `git clone git@github.com-lorenAtInnovise:goinnovise/<emplyee-name>.git`.
3. `cd <employee-name>`
4. `git checkout master`
5. `git remote add upstream git@github.com-lorenAtInnovise:goinnovise/loren.git`
6. `git pull upstream master`
7. `git push -u origin master` The -u argument sets the origin master branch to the upstream branch for change tracking.
8. Go to repo settings and enable GitHub pages
9. Be sure to follow steps below, especially setting \_config.yml settings otherwise github pages can become corrupted.

You can later update your downstream resumes with:
`git fetch upstream`
`git rebase upstream/master`

- Update `assets/images/profile.png`
- Update `assets/_config.yml`
- Update data.yml for the new employee.
