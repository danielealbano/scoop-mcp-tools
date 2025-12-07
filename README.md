# Scoop MCP Tools Bucket

[![Tests](https://github.com/danielealbano/scoop-mcp-tools/actions/workflows/ci.yml/badge.svg)](https://github.com/danielealbano/scoop-mcp-tools/actions/workflows/ci.yml)
[![Excavator](https://github.com/danielealbano/scoop-mcp-tools/actions/workflows/excavator.yml/badge.svg)](https://github.com/danielealbano/scoop-mcp-tools/actions/workflows/excavator.yml)

This is a custom [Scoop](https://scoop.sh) bucket that ships MCP-related tools, primarily for integrating Azure DevOps with Model Context Protocol (MCP) clients.

Currently included:

- `mcp-for-azure-devops-boards`  
  MCP server that exposes Azure DevOps Boards to MCP clients.

---

## Installation

First, add this bucket:

```powershell
scoop bucket add mcp-tools https://github.com/danielealbano/scoop-mcp-tools
````

Then install the Azure DevOps Boards MCP server:

```powershell
scoop install mcp-tools/mcp-for-azure-devops-boards
```

After installation you can run:

```powershell
mcp-for-azure-devops-boards --help
```

---

## Available manifests

| Manifest name                 | Command                       | Description                                         |
| ----------------------------- | ----------------------------- | --------------------------------------------------- |
| `mcp-for-azure-devops-boards` | `mcp-for-azure-devops-boards` | MCP server exposing Azure DevOps Boards to clients. |

More MCP-related tools may be added over time.

---

## Updating

To update the bucket and installed apps:

```powershell
scoop update
scoop update mcp-for-azure-devops-boards
```

---

## Contributing

If you want to add or improve manifests in this bucket:

1. Fork this repository.
2. Add or edit JSON manifests under the `bucket` directory.
3. Run the tests locally if you have the Scoop test harness available.
4. Open a Pull Request.

For general guidance on Scoop manifests, see:

* [Scoop App Manifests](https://github.com/ScoopInstaller/Scoop/wiki/App-Manifests)
* [Contributing Guide](https://github.com/ScoopInstaller/.github/blob/main/.github/CONTRIBUTING.md)

---

## License

Unless stated otherwise in individual manifests, this bucket’s contents are provided under the same license as the upstream projects.
The `mcp-for-azure-devops-boards` project itself is licensed under MIT:
[https://github.com/danielealbano/mcp-for-azure-devops-boards](https://github.com/danielealbano/mcp-for-azure-devops-boards)
