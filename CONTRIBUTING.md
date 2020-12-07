# Links

- [Create ticket and branch](#create-ticket-and-branch)
- [Deploying](#Deploying)

## How to contribute

If you'd like to contribute, start by searching through the [issues](https://github.com/SunriseProductions/ChoreoFX/issues) and [pull requests](https://github.com/SunriseProductions/ChoreoFX/pulls) to see whether someone else has raised a similar idea or question.

If you don't see your idea listed, and you think it fits into the goals of this library, do one of the following:
* **If your contribution is minor,** such as a typo fix, open a pull request.
* **If your contribution is major,** such as a new layer/node, start by opening an issue first. That way, other people can weigh in on the discussion before you do any work.

### Pull Requests

PRs to our libraries are always welcome and can be a quick way to get your fix or improvement slated for the next release. In general, PRs should:

- Only fix/add the functionality in question **OR** address wide-spread whitespace/style issues, not both.
- Add unit or integration tests for fixed or changed functionality (if a test suite already exists).
- Address a single concern in the least number of changed lines as possible.
- Include documentation in the repo or on our [docs site](https://auth0.com/docs).
- Be accompanied by a complete Pull Request template (loaded automatically when a PR is created).

For changes that address core functionality or would require breaking changes (e.g. a major release), it's best to open an Issue to discuss your proposal first. This is not required but can save time creating and reviewing changes.

In general, we follow the ["fork-and-pull" Git workflow](https://github.com/susam/gitpr)

1. Fork the repository to your own Github account
2. Clone the project to your machine
3. Create a branch locally along the naming convention we use below
4. Commit changes to the branch
5. Make sure that any otls adhere to the guidelines set below
6. Push changes to your fork
7. Open a PR in our repository and follow the PR template so that we can efficiently review the changes.

# Create ticket and branch
We use a git flow workflow. If you are unfamiliar with this have a look here:
https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow

We want to track all our activity through git hub's projects. Create an issue on one of our projects describing your issues, and then a branch based off the issue name. Push the branch in order to reserve it.


# Creating a new Layer
Use the following convention for labelling, nxt graph names:
    

    <pxr>_<usd>_<formattedname>.nxt
    
    Example:
    pxr_usd_class.nxt

# Creating a new node
Use the following convention for labelling, nxt node names:
    
    <FormattedName>

    Example:
    GetPrimFromAsset


#### Create a example layer for the library

Please see [Examples](examples)

# Deploying 

Only repo admins can deploy and make releases. You can follow the steps below on your own fork if you would like to mirror our release procedure.

All new layers/node should have an example.nxt to show a use case
