# moment.js
Packages repo of [Moment.js](http://momentjs.com/)

this is a repo to hold different versions of moment.js you may need
and also to make them available for the application as default

# Quick setup for new versions
    - git checkout master
    - git checkout -b v1-2-3 (Your new version to add or check for
      existing: git branch -a)
    - download your version somewhere
    - mkdir v1.2.3
    - cd v1.2.3/
    - Place your new files here
    - git add --all
    - git commit -m 'Adds version v1.2.3'
    - git push
    - done!
    - Make application wide available?
    - git checkout packages
    - git merge v1-2-3
    - git push
    - done!


# moment.js ready to run files
Downloaded from moment.js.org and set to the "packages" branch.

Checkout the single version (branch) you need or
create a new branch starting at the master branch and add your version as follow
    git co master
    git co -b myNewVersion (eg. v3-1-2; branches with slashes, folders with dots)
    mkdir ./v3.1.2/
and put your files here ./v3.1.2/*

The master branch should only contain the README to guide developers.
The "packages" branch should contain all versions to be used (old and new ones to have always
a fallback if older applications are not upgraded!).
The versioned branches are used to fix bugs, to improve or to use just as single branch 
for other projects.

If you use a versioned branch everywhere or in many projects, then merge this version into 
the "packages" branch.  But NEVER to the master!

The versioned branches can have their own README with more detailed information.


