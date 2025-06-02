# tao-code-quality

Repository to store code quality checks to help on CI validation, including CodeRabbitAI schemas

# How to contribute?

- Please open a PR adding or adapting a standard, pointing to the `main` branch.
- Make sure the changes are tested against another application using this repository. Please add that PR also in the description.
- Once the PR is approved and merged to `main`, the change will be available to all places using it.

# How to include CodeRabbit AI in your repositories

To use shared configuration, you need to:

- Create a `.coderabbit.yaml` file in the root of your repository with the following content:

```yaml
remote_config:
  url: "https://github.com/oat-sa/tao-code-quality/blob/main/coderabbit/js/be/v1/.coderabbit.yaml"
```
