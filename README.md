<div align="center">
  <img alt="VORAN Logo" src="assets/voran-logo.png" width="520">
</div>

<div align="center">
  <h3>VORAN AI application platform</h3>
  <p>Branded distribution of a mature LLM application codebase, prepared for VORAN.</p>
</div>

## Overview

This repository has been repackaged for `VORAN`.

The branding, top-level documentation, maintainer identity, and package metadata have been updated to present the project as a `VORAN` distribution. To keep the codebase stable and easy to run, the underlying Python package names, import paths, and compatibility-sensitive runtime identifiers remain unchanged.

## Compatibility Promise

- Existing package names such as `langchain`, `langchain-core`, and partner packages are preserved.
- Existing Python imports remain unchanged.
- Compatibility-sensitive environment variables and runtime endpoints are intentionally left as-is.
- This means you get `VORAN` branding without breaking the upstream developer experience.

## Quickstart

```bash
pip install langchain
# or
uv add langchain
```

```python
from langchain.chat_models import init_chat_model

model = init_chat_model("openai:gpt-5.4")
result = model.invoke("Hello, world!")
```

## Repository Layout

```txt
libs/core/             # Core primitives and abstractions
libs/langchain/        # Classic compatibility package
libs/langchain_v1/     # Primary package published as `langchain`
libs/partners/         # Third-party integrations maintained in this distribution
libs/standard-tests/   # Shared integration test suite
libs/text-splitters/   # Text chunking utilities
libs/model-profiles/   # Model profile refresh tooling
```

## Branding Scope

This repackaging focuses on visible branding layers:

- `README.md` and package-level documentation
- `LICENSE` copyright holders
- `pyproject.toml` display metadata and support links
- citation and maintainer-facing metadata

It does not rename package directories, module paths, imports, or runtime compatibility markers.

## Maintainer

This branded distribution is maintained by `VORAN Team`.
