## Conventional Commits

The [Conventional Commits](https://www.conventionalcommits.org/) specification is a lightweight convention on top of commit messages. It provides an easy set of rules for creating an explicit commit history; which makes it easier to write automated tools on top of. This convention dovetails with SemVer, by describing the features, fixes, and breaking changes made in commit messages.

## How should I write my commits?

The commit message should be structured as follows:

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

## The most important prefixes you should have in mind are:

feat(xxx): :sparkles: Features your commit message
	
fix(xxx): :bug: Bug Fixes
	
docs(xxx): :book: Documentation

style: :gem: Styles

refactor: :package: Code Refactoring

perf(xxx): :rocket: Performance Improvements

test(xxx): :rotating_light: Tests

build(xxx): :construction_worker: Build

ci(xxx): :computer: Continuous Integration
    
chore(xxx): :ticket: Chores

revert(xxx): :back: Reverts

## Examples:
### Good commits:

```
> git commit -m "feat(lang): added polish language"
1 file changed, 1 insertion(+)
```

```
> git commit -m "fix: minor typos in code"
5 file changed, 3 insertion(+)
```


### Bad commits:
```
> git commit -m "Ugly commit"
Commit message not follow Conventional Commits
```

```
> git commit -m "feat Ugly commit version 2"
Commit message not follow Conventional Commits
```

### Why Use Conventional Commits

- Automatically generating CHANGELOGs.
- Automatically determining a semantic version bump (based on the types of commits landed).
- Communicating the nature of changes to teammates, the public, and other stakeholders.
- Triggering build and publish processes.
Making it easier for people to contribute to your projects, by allowing them to explore a more structured commit history.
