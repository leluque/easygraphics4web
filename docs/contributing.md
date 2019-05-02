# Contributing to EasyGraphics4Web

Contributions to EasyGraphics4Web are very welcome.

# Instructions for Logging Issues

## 1. Search for Duplicates

Search the existing issues before logging a new one.

Some search tips:
 * *Don't* restrict your search to only open issues. An issue with a title similar to yours may have been closed as a duplicate of one with a less-findable title.
 * Check for synonyms. For example, if your bug involves an interface, it likely also occurs with type aliases or classes.
 * Search for the title of the issue you're about to log. This sounds obvious but 80% of the time this is sufficient to find a duplicate when one exists.
 * Read more than the first page of results. Many bugs here use the same words so relevancy sorting is not particularly strong.
 * If you have a crash, search for the first few topmost function names shown in the call stack.

## 2. Did you find a bug?

When logging a bug, please be sure to include the following:
 * If at all possible, an *isolated* way to reproduce the behavior
 * The behavior you expect to see, and the actual behavior

## 3. Do you have a suggestion?

We also accept suggestions in the issue tracker.

In general, things we find useful when reviewing suggestions are:
* A description of the problem you're trying to solve
* An overview of the suggested solution
* Examples of how the suggestion would work in various places
  * Code examples showing e.g. "this would be an error, this wouldn't"
  * Code examples showing the generated JavaScript (if applicable)
* If relevant, precedent in other languages can be useful for establishing context and expected behavior

# Instructions for Contributing Code

## Tips

### Faster clones

In order to save some time, you might want to clone it without the repo's full history using `git clone --depth=1`.

## Contributing bug fixes

Easygraphics4Web is currently accepting contributions in the form of bug fixes. 

## Contributing features

Features (things that add new or improved functionality to EasyGraphics4Web) may be accepted, but will need to first be approved ([labelled "help wanted"] by a project maintainer) in the suggestion issue.

## Housekeeping

Your pull request should: 

* Include a description of what your change intends to do
* Be a child commit of a reasonably recent commit in the **master** branch 
    * Requests need not be a single commit, but should be a linear sequence of commits (i.e. no merge commits in your PR)
* It is desirable, but not necessary, for the tests to pass at each commit
* Have clear semantinc commit messages 
    * e.g. "fix: iterated type in for-await-of"
* Include adequate tests 
    * At least one test should fail in the absence of your non-test code changes. If your PR does not match this criteria, please specify why
    * Tests should include reasonable permutations of the target fix/change
    * Include baseline changes with your change
    * All changed code must have 100% code coverage
* To avoid line ending issues, set `autocrlf = input` and `whitespace = cr-at-eol` in your git configuration