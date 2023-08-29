# Adding to your tex project


First, add as submodule:


cd myTexProject


git submodule add git@github.com:rfabbri/bibs-fabbri.git bib  # or HTTPS if you prefer

# Locally I do: 

git submodule add ~/lib/doc/bib/bibs-fabbri-repo bib  # or HTTPS if you prefer


git commit -am 'Add bibs-fabbri module'

git push origin master

## Working

Make a new change, say to REDME.md

### Pushint to upstream

gg add README.md
git commit -am 'minor readme changes'
git push

### Pulling from upstream

chdir to toplevel project folder
git submodule update --remote --merge

### Collaborator cloned your repo, bib/ is empty

git submodule update --init --recursive

## Moure about submodules

https://git-scm.com/book/en/v2/Git-Tools-Submodules

## Change remote of submodule
https://stackoverflow.com/questions/913701/how-to-change-the-remote-repository-for-a-git-submodule/914090#914090
