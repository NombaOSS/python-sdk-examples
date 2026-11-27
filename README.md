# Nomba Python SDK examples

Example server-side Python apps that show how to integrate with [Nomba](https://nomba.com) using the official [Nomba Python SDK](https://github.com/NombaOSS/nomba-python-sdk) (`nomba` on PyPI).

This repository holds **examples only**. The SDK itself lives at [NombaOSS/nomba-python-sdk](https://github.com/NombaOSS/nomba-python-sdk); report SDK bugs there.

## Layout

Each example is a self-contained app in its own top-level folder, with:

- a `pyproject.toml` and a committed `uv.lock` ([uv](https://docs.astral.sh/uv/));
- a `README.md` explaining what it demonstrates and how to run it;
- a `.env.example` listing the variables it needs, with no real values.

CI installs each example with `uv sync --locked` on Python 3.12, 3.13 and 3.14, then runs Ruff, mypy and pytest if the example includes them.

## Credentials

Examples read Nomba credentials from environment variables. Use **sandbox** credentials from the Nomba dashboard, and never commit a `.env` file, real keys or account IDs. CI never has access to Nomba credentials.

## Contributing

See the [NombaOSS contributing guide](https://github.com/NombaOSS/.github/blob/main/CONTRIBUTING.md) and [security policy](https://github.com/NombaOSS/.github/blob/main/SECURITY.md). Pull requests need a passing CI run and a review from [@NombaOSS/maintainers](CODEOWNERS).

## License

[MIT](LICENSE)

