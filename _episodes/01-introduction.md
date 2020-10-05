---
title: "Introduction to Development Practices"
teaching: 10
exercises: 40
questions:
- "What should I know to write better code?"
objectives:
- "Describe the barriers to writing good code."
- "Explain technical debt and how it occurs."
- "Describe the benefits of maintainable code."
- "Identify common problems with code."
keypoints:
- "Always assume code you write will be used by others (including a future version of yourself)."
- "Be critical of your own code, and that of others before you use it."
- "With maintainable code, prevention is better (and cheaper) than cure."
- "Find the right balance between adopting practices and research progress."
---

See topic [video lecture](FIXME).

> ## Action Stations!
>
> Imagine your project leader tells you that, quite unexpectedly, some important external collaborators are keen to work with and contribute to the development of some software developed by your group to meet some new, exciting, and potentially publication lucrative, research goals. The software has already been stored within a GitHub repository as a first step to sharing the code, but the software needs to be made suitable for collaboration and it's become obvious the software has a long way to go to be ready.
>
> In your assigned groups, take a look at the GitHub code repository at <https://github.com/softwaresaved/rf4>. Examine the contents of the repository (code, documentation, other assets) and as a group discuss what needs to be improved to get the software ready for your collaborators to understand it and contribute changes to it. Make a list of issues on what would make it difficult to use, install, maintain, extend, and generally collaborate, with this software. What would be the top three things you would address first and why?
>
> Make notes on your findings, and then briefly report back the top three things to the class. For a maximum of three minutes, for each of the three issues you found (i.e. a minute each), report back the following:
>
> 1. A few sentences description of the issue you found and how it affects users and/or developers.
> 2. A few sentences on how you would improve this issue for those users and/or developers.
>
> > ## Solution
> > #### Repository itself
> > - Repo name is unhelpful rf4
> > - The README.md mentions this code has been developed since 2010, but the commits indicate it's only just been committed to GitHub
> > - No CITATION file
> > - LICENSE file is empty
> > - Commits with cursory commit messages (e.g. 'Change', 'Not working')
> > - Code is not in a working state on master branch - developing code should either be on a separate branch, or file releases made available with versions
> > - No tests
> > - GitHub has highlighted potential security vulnerabilities with the repo's dependencies
> >
> > #### README.md
> > - No prerequisites
> > - No instructions for running the code
> > - No description of the data used by the software that is in the repository
> > - Incomplete description of the repository data directory
> > - Links to blog post that isn't there
> >
> > #### What questions do we want to answer with this data?
> > - No real content, comment that says it'll be finished later
> >
> > #### Code
> > - Arbitrary copy of the .py with a _working suffix, no explanation
> > - Many function docstrings missing (including key functions)
> > - Inconsistent commenting of logger throughout
> > - Logger retrieved in each function (and sometimes not used), when it could be done once and referenced later
> > - Hard coded file path references inline
> > - print(len(df)) with no context, comment - why isn't it logged?
> > - Commenting good in places, nonexistent commenting in others
> > - Many variable names are non-descriptive single letters
> > - The code doesn't work! (df renamed to df47 in main()
> > - The main() function is overlong and uncommented
> > - Commented out function
> > - Two functions have a number in the function name without explanation
> > - Too many spaces in add_column5 function inconsistent with coding style
> > - Some ultra-long code lines that should be properly formatted over multiple lines
> {: .solution}
{: .challenge}

{% include links.md %}

