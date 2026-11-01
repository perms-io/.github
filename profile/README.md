<p align="center">
  <a href="https://perms.io">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="assets/logo-dark-mode.svg">
      <img src="assets/logo-light-mode.svg" alt="Permio" width="360">
    </picture>
  </a>
</p>

<p align="center">
  <strong>RBAC and fine-grained authorization as a service.</strong><br>
  Define permissions and roles, grant them on hierarchical resources, and check access in one API call.
</p>

<p align="center">
  <a href="https://perms.io">Website</a> ·
  <a href="https://docs.perms.io">Docs</a> ·
  <a href="https://app.perms.io">Dashboard</a>
</p>

---

Grant roles to your users on resource URIs such as `/projects/p1/docs/42`, then ask
"may this principal do X on this resource?". Built for multi-tenant apps.

```ts
import { Permio, resource } from "permio";

const permio = new Permio({ apiKey: process.env.PERMIO_API_KEY!, project: "my-app" });

const allowed = await permio.check({
  principal: "alice",
  resource: resource("docs", 42), // "/docs/42"
  permission: "docs.read",
});
```

## 📦 SDKs

| Language | Install | Repository |
| --- | --- | --- |
| TypeScript / JavaScript | `npm install permio` | [permio-js](https://github.com/perms-io/permio-js) |
| Python | `pip install permio` | [permio-python](https://github.com/perms-io/permio-python) |
| Go | `go get github.com/perms-io/permio-go@latest` | [permio-go](https://github.com/perms-io/permio-go) |
| Rust | `cargo add permio` | [permio-rust](https://github.com/perms-io/permio-rust) |
| Java | `io.perms:permio` (Maven Central) | [permio-java](https://github.com/perms-io/permio-java) |

## 🛠️ Tools

| Tool | Get it |
| --- | --- |
| CLI | `npm install -g permio-cli` or `brew install perms-io/tap/permio` |
| MCP server for AI assistants | `https://mcp.perms.io/mcp` |
| Terraform provider | [terraform-provider-permio](https://github.com/perms-io/terraform-provider-permio) |
