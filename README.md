# Google OSS Complier MCP Server (`/google-oss`)

An MCP (Multi-Capability Provider) server for the Gemini CLI that helps make projects compliant with Google's open-source standards.

## Overview

This server provides a `/google-oss` tool that generates a detailed prompt. This prompt instructs the Gemini CLI to perform the necessary steps to ensure a project meets Google's open-source requirements, such as adding a `LICENSE` file, a `CONTRIBUTING.md`, and appropriate source headers.

## Installation

The recommended installation method is using the `fastmcp` command-line tool.

1.  **Clone this repository:**
    ```bash
    git clone https://github.com/ksprashu/gemini-cli-mcp-google-oss.git
    cd gemini-cli-mcp-google-oss
    ```

2.  **Install into Gemini CLI:**
    ```bash
    fastmcp install gemini-cli main.py --name google-oss
    ```

## Usage

Once installed, you can use the tool directly from the Gemini CLI:

```
> /google-oss
```

## Development

This project uses `uv` for dependency management.

```bash
uv venv
source .venv/bin/activate
uv pip install -e .
```

## Disclaimer

This is not an officially supported Google product.

## License

This project is licensed under the Apache License, Version 2.0. See the [LICENSE](LICENSE) file for details.
