# Permio

[Permio](https://perms.io) is RBAC and fine-grained authorization as a service.
Define permissions and roles, grant them to your users on hierarchical resource
URIs such as `/projects/p1/docs/42`, and ask "may this principal do X on this
resource?" in one API call. Built for multi-tenant apps.

- **Website:** [perms.io](https://perms.io)
- **Docs:** [docs.perms.io](https://docs.perms.io)
- **Dashboard:** [app.perms.io](https://app.perms.io)

## SDKs

| Language | Install | Repository |
| --- | --- | --- |
| TypeScript / JavaScript | `npm install permio` | [permio-js](https://github.com/PrivateJAR/permio-js) |
| Python | `pip install permio` | [permio-python](https://github.com/PrivateJAR/permio-python) |
| Go | `go get github.com/PrivateJAR/permio-go@latest` | [permio-go](https://github.com/PrivateJAR/permio-go) |
| Rust | `cargo add permio` | [permio-rust](https://github.com/PrivateJAR/permio-rust) |
| Java | `io.perms:permio` (Maven Central) | [permio-java](https://github.com/PrivateJAR/permio-java) |

## Tools

- **CLI:** `npm install -g permio-cli` or `brew install PrivateJAR/tap/permio`
- **MCP server** for AI assistants: `https://mcp.perms.io/mcp`
