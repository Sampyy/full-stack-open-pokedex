Implementing CI/CD in Ruby for a team of about 6 people could include some of the tools discussed ahead.

The leading linting solution for Ruby seems to be RuboCop, which can check the code and also automatically correct code offences and format the code. There are tools (such as https://github.com/AtomLinter/linter-rubocop) to implement RuboCop and several other Ruby linters to the CI/CD pipeline.

For testing, we could use a testing framework such as RSpec to implement tests. We could then set these to run automatically on commit if using for example github actions, or Semaphore.

For setting up the CI environment locally, the best option will be Jenkins. For cloud-based CI environments there are multiple options, such as GitHub Actions, CloudBees and CircleCI, the earlier mentioned Semaphore is also an option.

With a small team of 6, a cloud-based environment would likely be a better fit. Their cost usually scales with usage, and with a small team the cost will likely be cheaper compared to running a locally based one, and it is also much simpler to setup and keep running. It does depend on what kind of an application the team is making though, if it is very heavy to run, or requires some specific hardware requirements, then a local self-hosted environment might be the only option, since cloud-based environments are often a bit limited on what they can run.
