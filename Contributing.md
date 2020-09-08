# Contributing Guidelines

Before adding anything to the project, make sure to follow the following steps

# 1. Check Out a New Branch

Whenever you are working on a new post or site change, make sure to checkout a 
new branching using git.

```bash
git checkout -b $branch_name
```

# 2. Test Your Code

Make sure to view your addition in a browser. Make sure all dates
and various details are up to date and correct.

View the website using the following commands:
```bash
# May need to execute `bundle update` or `bundle install` to ensure
# that you have up to date plugins and execution
bundler exec jekyll serve
```

# 3. Make a Pull Request

Do not push directly to the main branch, instead make a pull request
and have it reviewed by other contributors, then commit it to the repository.
If you're not sure about a feature, you can make the PR as a draft before 
having it ready to submit. 
