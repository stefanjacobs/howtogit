# How to GIT

My personal collection of How To Git ;-)

## Show remotes

    git remote -v

## Creating a remote repository from command line

    # Create local git repository
    echo "# keycloak_min" >> README.md
    git init
    git add README.md
    git commit -m "first commit"

    # Create remote repository
    curl -u 'stefanjacobs' https://api.github.com/user/repos -d '{"name":"keycloak_min"}'

    # Link local repository to remote repository
    git remote add origin git@github.com:stefanjacobs/keycloak_min.git
    git push -u origin master

## Adding a remote repository

    git remote add github git@github.com:stefanjacobs/<reponame>.git
    git push github master

## Setting upstream repository

    git push -u github master
