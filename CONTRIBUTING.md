# Contributing to `fiftyone-examples`

FiftyOne is open source and community contributions are welcome!

## Setup

If you are contributing new material to this repository, please install the
pre-commit hooks so that your changes will be passed through our linting tools:

```
pre-commit install
```

## Issues

FiftyOne defines four categories of issues:
-   Feature requests
-   Bug reports
-   Documentation fixes
-   Installation issues.

Details about each issue type and the issue lifecycle are discussed in the
[FiftyOne Issue Policy](ISSUE_POLICY.md).

## Bugfixes and improvements

Feel free to submit bugfixes or improvements to existing examples by sending us
a pull request.

## Adding a new example

Contributing a new example to the repository is easy:

-   Add your example as a [Jupyter Notebook](https://jupyter.org) to the
    `examples/` folder
-   Add an entry for your example to `index.yaml`
-   Run the make script, which will add links in a new cell at the beginning of
    your notebook and add your notebook to the table of contents in
    `README.md`:

```shell
python scripts/make_examples.py examples/your_example_notebook.ipynb
```

-   Submit your changes as a pull request

Check out the notebook templates in `templates/` to get started writing a new
example.
