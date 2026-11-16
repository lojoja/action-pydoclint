# action-pydoclint

A composite action that lints docstrings with [pydoclint](https://jsh9.github.io/pydoclint).

This repository is not meant to be referenced in third-party workflows; please fork the repository if you would like to use it in your project.

## Inputs

| Name              | Description                                       | Required | Default |
| ----------------- | ------------------------------------------------- | :------: | ------- |
| cache             | Whether to cache project dependencies.            |          | "true"  |
| package_manager   | The package manager to use ("poetry" or "uv").    |          | "uv"    |
| python_version    | The python version to use in SemVer range syntax. |          | "3.14"  |
| working_directory | The working directory for the action.             |          | "."     |

## Examples

```
jobs:
  pydoclint:
    runs-on: ubuntu-latest
    steps:
      - uses: lojoja/action-pydoclint@main
        with:
          cache: "true"
          package_manager: uv
          python_version: "3.14"
```

## License

action-pydoclint is released under the [MIT License](./LICENSE)
