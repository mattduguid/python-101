# libraries

## for GitHub API interactions

### source

- https://github.com/PyGithub/PyGithub

### install

```bash
pip install pygithub

```

### example

```python
from github import Github

g = Github("your_personal_access_token")
repo = g.get_repo("your-username/your-repo")
issues = repo.get_issues(state="open")

for issue in issues:
    print(issue.title)
```

## for local Git repo operations (library)

### source

- https://github.com/gitpython-developers/GitPython

### install

```bash
pip install gitpython
```

### example

```python
from git import Repo

repo = Repo("/path/to/repo")
repo.git.pull()
print(repo.head.commit.hexsha)
```

## for local Git repo operations (raw)

### example

```python
import subprocess

subprocess.run(["git", "clone", "https://github.com/your/repo.git"])
```
