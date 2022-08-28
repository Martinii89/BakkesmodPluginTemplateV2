# Setup

## Create a repository from this template

1. Click the big green button `Use this template` or click <a href="../../generate">here</a>.
1. Enter a Repository name and click `Create repository from template`
1. Head over to the created repository and complete the setup.

## Configure the repository so workflows can be added automatically

1. In a new browser tab, go to [the token settings page of your account](https://github.com/settings/tokens).
1. Click "generate new token".
1. Assign any name like "workflow token", click the "workflow" check box (which will automatically select everything under "repo" as well), then scroll down and click "Generate token".
1. Copy the token by clicking the icon with the two overlapping squares.
1. In the other browser tab with your repository, click Settings -> Secrets -> Actions.
1. Set the name of the secret to `REPO_SETUP_TOKEN` and paste the token, then click "Add secret"

## Complete setup

1. In the a new repository, <a href="../../edit/master/cookiecutter.json">complete the project setup</a> by editing the `cookiecutter.json` file. 
1. Hit <kbd>cmd</kbd> + <kbd>S</kbd> and then <kbd>Enter</kbd> to perform a commit (the commit message doesn't really matter).
1. Wait <a href="../../actions">Setup Repository Action</a> to complete.
1. That's it, easy isn't it?

If you have anything to add, please reply in this [Twitter thread]().

## Automated builds
Builds and releases can be automated using GitHub Actions.  Tagging a commit with a version tag will trigger a release.

```bash
git commit v1.0.0 -m "Release message here!"
git push --tags
```

---
# What is this all about?

On June 6, 2019, [GitHub introduced Repository Templates](https://github.blog/2019-06-06-generate-new-repositories-with-repository-templates/) giving users an easy way to share boilerplate for their projects. This feature is fantastic, but lacking adoption to my knowledge and opinion for one reason... [Read the full blog post](https://stefanbuck.com/blog/repository-templates-meets-github-actions) to learn how to template new projects using repository templates and GitHub Actions.
