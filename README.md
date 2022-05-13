# Assumptions
- You're on macos so you're using zsh
- You have brew setup already because you needed brew to install ansible
- You've setup access token in gitlab
- You've setup your ssh in bitbucket and gitlab

# Roadmap
1. General tooling
  - Node via nvm, nvm auto switching, docker, sam, yarn
  - optional? oh my zsh
2. Repos
  - Install all the repos, with custom logic where required
3. Nices to have's if possible
  - gitlab token and ssh generationt

## Oh my zsh
- [1] Optional?
- [6] nvmrc switching automatic plugin, maybe instead I could use a custom script that I can insert into zshrc

## Repos
- Loop through repos instead of doing one at a time
- Should check if repo is already setup and skip if it is?

## Brew
- Issue with the assumption that we have brew installed is that brew might be
 installing incorrect arch programs on m1 chips
- Investigate what arch brew is installed if you have m1 ???
- Check installing docker from brew

## Tokens / SSH / Access token
- [8] It'd be nice if there was a warning at the start to say hey you don't have
  your access tokens setup I could check if your ssh-keygen is generated and when
  something fails I could say your ssh might not be setup
- Might look into this in the future
- https://docs.gitlab.com/ee/api/users.html#create-a-personal-access-token
- https://docs.gitlab.com/ee/api/users.html#add-ssh-key-for-user
- also look into seeing if there is a way to check if ssh is setup

## Docker
- [4] for arm need to fetch docker from site, otherwise install via brew ( this will need some work )

## AWS SAM CLI
- [5] need to install this after docker via brew

## Yarn
- [3] Need to install yarn as well

## Ansible queries
- [1] Can we have optionally selected tasks
- [1.1] NPM_TOKEN || ssh aren't set then just fail
- [2] Tags for uninstalling possibly
- [7] How to structure multiple repos, thinking to put each repo into it's only file
-

# TODO

## Insomnia
- look into installing and importing insomnia files

## Update everything with readmes
