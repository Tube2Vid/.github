# Contributing to Tube2Vid

Thanks for helping improve the Tube2Vid SDKs, CLI, MCP server and API spec. These guidelines apply to every repository in the [Tube2Vid organization](https://github.com/Tube2Vid) unless a repository has its own `CONTRIBUTING.md`.

## Before you start

- **Bugs and feature requests:** open an issue with the templates provided. Search existing issues first.
- **Download failures on a specific site** (a YouTube or TikTok link that will not download) are usually server-side, not SDK bugs. Check the [platform status page](https://tube2vid.com/status) and contact [support](https://tube2vid.com/help) instead of opening an SDK issue.
- **Security problems:** do not open an issue. See [SECURITY.md](SECURITY.md).
- For larger changes, open an issue to discuss the approach before writing code.

## Pull requests

1. Fork the repository and create a branch from `main`.
2. Keep the change focused. One fix or feature per pull request.
3. Add or update tests. Tests must not hit the network or need a real API key; use the fake HTTP server or transport the repository already uses.
4. Run the repository's test command (see its README) and make sure CI passes.
5. Update the README and `CHANGELOG.md` when behaviour changes.

The SDKs mirror one another and the [OpenAPI spec](https://github.com/Tube2Vid/api). If you add a method to one SDK, mention it in the issue so the others can follow.

## Code of conduct

Everyone taking part is expected to follow the [Code of Conduct](CODE_OF_CONDUCT.md).

## License

By contributing you agree that your contributions are licensed under the MIT license of the repository you contribute to.
