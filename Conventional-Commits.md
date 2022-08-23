# Conventional Commits

The [Conventional Commits](https://www.conventionalcommits.org/) specification is a lightweight convention on top of commit messages. It provides an easy set of rules for creating an explicit commit history; which makes it easier to write automated tools on top of. This convention dovetails with [SemVer](https://semver.org/), by describing the features, fixes, and breaking changes made in commit messages.

## How should I write my commits?

Conventional Commits have the following format:

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

``
feat!:, or fix!:, refactor!:, etc., which represent a breaking change (indicated by the !) and will result in a SemVer major.
``

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

```
> git commit -m "build: updated the offline prod app version to v2.1.18 (#46897)"
4 file changed, 1 insertion(+)
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

### Why to use Conventional Commits?

- Automatically generating CHANGELOGs.
- Automatically determining a semantic version bump (based on the types of commits landed).
- Communicating the nature of changes to teammates, the public, and other stakeholders.
- Triggering build and publish processes.
Making it easier for people to contribute to your projects, by allowing them to explore a more structured commit history.


### NPM Packages
- [Commitizen](https://www.npmjs.com/package/commitizen)
- [Commitlint](https://commitlint.js.org/)

### Reference

- [To setup VSCode Conventional-Commits Extension](https://marketplace.visualstudio.com/items?itemName=vivaxy.vscode-conventional-commits)
- [Read more about Conventional Commits](https://medium.com/neudesic-innovation/conventional-commits-a-better-way-78d6785c2e08)
