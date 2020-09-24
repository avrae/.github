# Contributing

Thanks for taking the time to contribute to Avrae! 

## TL;DR

- Talk with us at [the dev Discord](https://support.avrae.io)!
- Use the [bugs project page](https://github.com/orgs/avrae/projects/4) and 
[feature request project page](https://github.com/orgs/avrae/projects/6) to choose an issue to work on. 

## Developing Avrae

Avrae is comprised of many different modules that interact in various different ways. We highly recommend hopping in the
[Avrae Development Discord](https://support.avrae.io) to chat with us and ask for help in #advanced-help!

### Bot Code Structure

If you're familiar with developing bots using discord.py, Avrae uses the cog system to organize commands into groups.
The top-level python module containing these cogs are `cogs5e` and `cogsmisc`, and top-level files in those modules
are where the commands themselves will be found. This is your best bet to getting started on a command!

### Limitations

Unfortunately, not all parts of Avrae are available to run locally - for example, we can't release the data of 
everything in 5e, and the D&D Beyond connection is closed source. Where possible, we have made it possible to run
Avrae without these components configured.

### Choosing an Issue

If you have a feature you want to implement that's not a currently open feature request, great!

If you're looking for an open issue to solve, bugs and feature requests are listed and prioritized at the
[bugs project page](https://github.com/orgs/avrae/projects/4) and 
[feature request project page](https://github.com/orgs/avrae/projects/6). Take a look at these first!

If you're a first time contributor to Avrae, we recommend taking a look for issues labelled `good first issue`! 
These issues provide an introduction to the bot's code base without having to be too familiar with the inner workings
of the bot.

### Code Style

Where possible, Avrae conforms to the standards set in [PEP 8](https://www.python.org/dev/peps/pep-0008/) (with a max
line length of 120 rather than 79).

## Opening a PR

When you're ready, go ahead and open a pull request! Each repository will include a PR template and checklist, so 
please fill that out! If your PR closes an issue, include the words `Resolves #123` in your summary for each issue.

Additionally, you might be asked to change the branch your PR points to, depending on the repository. Usually, this
will be the `master` or `main` branch, but in certain cases it may be `dev` or `20XXwYY`.

### Code Review

Feel free to request a review from other contributors! Usually, the main reviewer is @mommothazaz123, but anyone
is free to comment on open PRs.

During the code review process, a few things will happen on your PR. First, our automated checks will run:
- Travis CI: Basic code functionality test. If you get a red X on this one, follow the link to see what happened!
- CodeCov: PR test coverage. Don't worry if you get a red X on this one.

After that, project maintainers will give feedback and leave reviews. Once your PR has received at least 1 approval from
maintainers and has no requested changes, it's good to go! A maintainer will merge it into the main repository soon.

## After Merge

If your PR closes an issue with an assigned priority of P4 or above, you'll be given a special role in the development
Discord, access to a secret channel, and a shoutout in the changelog!
