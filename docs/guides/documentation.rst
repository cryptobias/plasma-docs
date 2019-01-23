# Guidelines for Writing Documentation
This is a basic set of guidelines that we at PG use to write our documentation.
This page, like all of our documentation, is a living document and subject to a lot of change!
If you have suggestions for these guidelines, feel free to create an issue or open a pull request.

## reStructuredText
PG projects currently use [Read the Docs](https://readthedocs.org/), a powerful documentation generator, to build and display documentation.
*Read the Docs* uses the [reStructuredText](http://docutils.sourceforge.net/rst.html) markup language 
We've provided some documentation on how to use reStructuredText as well as some of the reStructuredText styles we use [here](TODO).

## Things to Document
1. Any new features that you've added.

New features are constantly being added to our projects, so it's important that our documentation stays up to date with these features.
Otherwise, it'll be really hard for other developers to discover and use these features!
The more discoverable a feature is, the more people will make use of all your hard work.

The best way to document new features is to find and update the relevant page in the `/docs` folder before you make a pull request.
If you're not sure which pages should be updated, feel free to ask and another community member will link you to the right pages.

2. Any changes you've made that break or change an old feature.

Sometimes new updates break old features in important ways.
Maybe the format of data coming out of a function is different, maybe the function takes different parameters.
Either way, it's important that these changes are documented so developers know how to use the new functionality.

3. Any design choices that aren't immediately obvious.

As projects get bigger and bigger, they become increasingly more architecturally complex.
It's important to manage this complexity by documenting both the architecture and the processes that led to deciding on that architecture.
Not only does this make things easier for future developers, but it also makes clear that the PG projects are living organisms.
Documented decision processes allows someone to more effectively question a design instead of assuming that there must've been certain reasons that one route was taken over another.

## Style Guide
1. Keep documentation simple.

Documentation should be as simple as possible.
After a few months, you start to forget things about documentation and code that *you* wrote.
Strong, understandable, and simple documentation is important for ensuring that you or others can dive into the code as quickly as possible.
Remember documentation isn't just for yourself, it's for other people who might not have any of the background knowledge that you do.

2. Reuse documentation.

With brevity comes simplicity, so try to keep your documentation as short as possible without sacrificing quality.
To avoid long articles, link out to other pages and provide background detail when necessary.
Think of documentation pages like Wikipedia pages - assume that the reader has no background knowledge but also assume that they're willing to go read other pages that already exist.

3. Keep paragraphs short.

Long paragraphs are difficult to read and often contain too much irrelevant information.
Don't make paragraphs longer than they need to be.
Each paragraph should contain a small set of relevant information that conveys a central idea.
If you're conveying many ideas per paragraph, you probably want to break things out into more paragraphs.

4. Put each sentence on a separate line.

This unusual style requirement becomes extremely helpful when using version control systems.
Whenever you make a pull request to change documentation, reviewers will look at the change by checking the "diff", or difference between the old and new files.
For an example of a diff, check out [this](https://github.com/octocat/linguist/compare/master...octocat:an-example-comparison-for-docs) page by GitHub.

When sentences are on the same line, diffs are very hard to read.
A change in a sentence in the middle of a large paragraph might make the reviewer scroll very far to find what's been changed.
When each sentence is on a different line, the review can easily see what's been modified.
Best of all, your paragraphs won't be broken apart on the actual docs page.

5. Use code examples to illuminate, not to handwave.

Well-placed code examples can be extremely helpful in explaining a topic.
Often, examples can explain a feature better than language can.
However, it's important that you don't use code examples to *avoid* explaining a topic.

