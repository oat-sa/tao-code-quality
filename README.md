# tao-code-quality

Repository to store code quality checks to help on CI validation, including CodeRabbitAI schemas

# How to contribute?

- Please open a PR adding or adapting a standard, pointing to the `main` branch.
- Make sure the changes are tested against another application using this repository. Please add that PR also in the description.
- Once the PR is approved and merged to `main`, the change will be available to all places using it.

## Introducing a new CodeRabbit standard

- Please respect the content structure:
  - coderabbit
    -  {language}
      - {subpath}
        - v1 (_version is required_)
          - .coderabbit.yaml
- Make sure to test that the standards are working as expected in the target repository

**IMPORTANT**: Please, avoid introducing new standards as much as possible, instead make the applications
comply to the existing standards as the goal is to _align development_, 
_reduce learning curve_, make _code more maintainable_ and _concise_. 

# How to include CodeRabbit AI in your repositories

To use shared configuration, you need to:

- Create a `.coderabbit.yaml` file in the root of your repository with the following content: 

```yaml
remote_config:
  url: "https://raw.githubusercontent.com/oat-sa/tao-code-quality/refs/heads/main/coderabbit/js/be/v1/.coderabbit.yaml"
```

*_In this example, we are pointing to a config for a JS and BE standards, as per `js/be/v1/.coderabbit.yaml` 
in the path, but you can choose among the available standards_.
