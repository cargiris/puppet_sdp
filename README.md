Table of Contents
=================

  * [Where Did All The Previous Code Go?](#where-did-all-the-previous-code-go)
  * [Copy This Repo Into Your Own Git Server](#copy-this-repo-into-your-own-git-server)
    * [GitHub](#github)

Created by [gh-md-toc](https://github.com/ekalinin/github-markdown-toc.go)

# Where Did All The Previous Code Go?

I am updating this README.md so it's apparent I've just used the template repo as a starting point.
For reference I used the instructions below to get started on my own control-repo.

# Copy This Repo Into Your Own Git Server

## GitHub

1. Prepare your local git client to authenticate with GitHub.com or a local GitHub Enterprise instance.
  - https://help.github.com/articles/generating-ssh-keys/
  - https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/

2. Create a repository called `control-repo` in your user account or organization.  Ensure that "Initialize this repository with a README" is not selected.
  - https://help.github.com/articles/creating-a-new-repository/

3. Make a note of your repository URL (HTTPS or SSH, depending on your security configuration).

4. Clone this control repository to your laptop/workstation:
  - `git clone <repository url>`
  - `cd control-repo`

5. Remove this repository as the origin remote:
  - `git remote remove origin`

6. Add your internal repository as the origin remote:
  - `git remote add origin <url of your github repository>`

7. Push the production branch of the repository from your machine up to your git server
  - `git push origin production`
