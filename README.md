# rimusa.github.io
Personal Website


## Downloading:

To download the repo and the private version, use the following code block:

```
cd ~/Downloads
git clone https://github.com/rimusa/rimusa.github.io.git
cd rimusa.github.io
git remote add private-remote [PRIVATE URL]
git fetch -u private-remote private-branch:private-branch
git fetch -u private-remote changes-hobbies:changes-hobbies
git fetch -u private-remote changes-cv:changes-cv
git fetch -u origin changes:changes
```


## Run Locally

To run locally, use the following code block:

```
cd docs/
bundle install
bundle exec jekyll serve
```