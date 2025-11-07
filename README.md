# Google OSS Compliance Extension for Gemini CLI

A Gemini CLI extension that helps make projects compliant with Google's open-source standards.

## Overview

This extension provides the `/make-google-oss` command. This command generates a detailed, step-by-step plan for the Gemini CLI to ensure a project meets Google's open-source requirements, including:
- Adding a `LICENSE` file (Apache 2.0).
- Adding a `CONTRIBUTING.md` file.
- Adding Apache 2.0 license headers to all source code files.
- Updating the `README.md` with required disclaimers and license information.

## Installation

To install this extension, use the `gemini` command:

```bash
gemini extensions install https://github.com/ksprashu/gemini-cli-mcp-google-oss
```

## Usage

Once installed, you can use the command directly from the Gemini CLI:

```
> /make-google-oss
```

The agent will then:
1.  Acknowledge the current working directory.
2.  Clone a reference template.
3.  Copy core files (`LICENSE`, `CONTRIBUTING.md`).
4.  Apply license headers to source files.
5.  Update the `README.md`.
6.  Clean up temporary files.

It will provide a live progress tracker as it executes these steps.

## Disclaimer

This is not an officially supported Google product.

## License

This project is licensed under the Apache License, Version 2.0. See the [LICENSE](LICENSE) file for details.