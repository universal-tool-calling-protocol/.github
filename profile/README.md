# Universal Tool Calling Protocol (UTCP)

<p align="center">
  <img src="../assets/banner.png" alt="UTCP Logo" />
</p>

<p align="center">
  <strong>A protocol that lets AI agents call any tool, over any channel—directly and without wrappers (unlike the MCP)</strong>
</p>

The **Universal Tool Calling Protocol (UTCP)** is an open standard, as an alternative to the MCP, that describes *how* to call existing tools rather than *proxying* those calls through a new server. After discovery, the agent speaks directly to the tool’s native endpoint (HTTP, gRPC, WebSocket, CLI, …), eliminating the “wrapper tax,” reducing latency, and letting you keep your existing auth, billing and security in place.

---

## Getting Started

* 📚 **Read the [Documentation](https://utcp.io)** for specs, examples and best practices
* 📜 **Read the [RFC](https://github.com/universal-tool-calling-protocol/utcp-specification/blob/main/RFC.md)** for the formal proposal,
* 🤖 **Play around with the [UTCP-agent](https://github.com/universal-tool-calling-protocol/utcp-agent) to prototype how the protocol works
* 💻 **Start building with our SDKs:**

  * [TypeScript SDK](https://github.com/universal-tool-calling-protocol/typescript-utcp)
  * [Python SDK](https://github.com/universal-tool-calling-protocol/python-utcp)
  * [Go SDK](https://github.com/universal-tool-calling-protocol/go-utcp)

---

## Project Structure

| Repository                                                                                    | Description                         | Stars                                                                                                                                                                                             |
| --------------------------------------------------------------------------------------------- | ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [`utcp-specification`](https://github.com/universal-tool-calling-protocol/utcp-specification) | Formal spec, RFC and reference docs | [![Stars](https://img.shields.io/github/stars/universal-tool-calling-protocol/utcp-specification?style=social)](https://github.com/universal-tool-calling-protocol/utcp-specification/stargazers) |
| [`python-utcp`](https://github.com/universal-tool-calling-protocol/python-utcp)               | Python implementation               | [![Stars](https://img.shields.io/github/stars/universal-tool-calling-protocol/python-utcp?style=social)](https://github.com/universal-tool-calling-protocol/python-utcp/stargazers)               |
| [`typescript-utcp`](https://github.com/universal-tool-calling-protocol/typescript-utcp)       | TypeScript implementation           | [![Stars](https://img.shields.io/github/stars/universal-tool-calling-protocol/typescript-utcp?style=social)](https://github.com/universal-tool-calling-protocol/typescript-utcp/stargazers)       |
| [`go-utcp`](https://github.com/universal-tool-calling-protocol/go-utcp)               | Go implementation                   | [![Stars](https://img.shields.io/github/stars/universal-tool-calling-protocol/go-utcp?style=social)](https://github.com/universal-tool-calling-protocol/go-utcp/stargazers)               |

---

## Contributing

We welcome issues, pull requests and design discussion. **If you’d like to add support for another language, tool or framework, open a discussion first so we can align on the design!**

---

## About

UTCP is an open‑source project released under the **MPL‑2.0** license and maintained by a growing community of AI‑tooling enthusiasts. If your organization relies on direct, low‑latency access to existing APIs—or if you simply dislike writing wrappers—we’d love to have you involved!

---

## UTCP vs MCP

### UTCP's Core principle: 
If humans can interact with an API, AI should be able to do the same with no change in the API and the same security guarantees.

### Core Requirements
* No wrapper tax: UTCP must be able to call any tool without requiring any changes to the tool itself or the infrastructure required to call it.
* No security tax: UTCP must be able to call any tool while guaranteeing the same security as if the tool was called by a human.
* Scalable: UTCP must be able to handle a large number of tools and calls.
* Simple: UTCP must be simple to implement and use.

<p align="center">
  <!-- TODO: Replace with animated demo once recorded -->
  <img src="../assets/utcp-vs-mcp.gif" alt="UTCP vs MCP Gif" />
</p>
