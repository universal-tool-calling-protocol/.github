# Universal Tool Calling Protocol (UTCP)

<p align="center">
  <img src="../assets/banner.png" alt="UTCP Logo" />
</p>

<p align="center">
  <strong>A protocol that lets AI agents call any native endpoint, over any channel - directly and without wrappers</strong>
</p>

The **Universal Tool Calling Protocol (UTCP)** is an open standard, as an alternative to the MCP, that describes *how* to call existing tools rather than *proxying* those calls through a new server. After discovery, the agent speaks directly to the tool’s native endpoint (HTTP, gRPC, WebSocket, CLI, …), eliminating the “wrapper tax,” reducing latency, and letting you keep your existing auth, billing and security in place.

---

## Getting Started

* 📚 **Read the [Documentation](https://utcp.io)** and **[RFC](https://github.com/universal-tool-calling-protocol/utcp-specification/blob/main/RFC.md)** for specs, examples and best practices
* 🤖 **Try the [UTCP Agent](https://github.com/universal-tool-calling-protocol/utcp-agent)** to prototype the protocol
  
* 🔌 **MCP users:** Run the **UTCP–MCP Bridge** to connect to +230 tools with only one MCP server → [`utcp-mcp`](https://github.com/universal-tool-calling-protocol/utcp-mcp) <!-- Update repo slug if different -->

---

## Project Structure (share a ⭐!)

| Repository                                                                                             | Description                                                | Stars                                                                                                                                                                                             |
| ------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [`utcp-specification`](https://github.com/universal-tool-calling-protocol/utcp-specification)          | Formal spec, RFC and reference docs                        | [![Stars](https://img.shields.io/github/stars/universal-tool-calling-protocol/utcp-specification?style=social)](https://github.com/universal-tool-calling-protocol/utcp-specification/)          |
| [`utcp-mcp`](https://github.com/universal-tool-calling-protocol/utcp-mcp)                | MCP server that lets you connect to any native endpoint, powered by UTCP   | [![Stars](https://img.shields.io/github/stars/universal-tool-calling-protocol/utcp-mcp?style=social)](https://github.com/universal-tool-calling-protocol/utcp-mcp/)                |
| [`python-utcp`](https://github.com/universal-tool-calling-protocol/python-utcp)                        | Python SDK                                      | [![Stars](https://img.shields.io/github/stars/universal-tool-calling-protocol/python-utcp?style=social)](https://github.com/universal-tool-calling-protocol/python-utcp/)                        |
| [`typescript-utcp`](https://github.com/universal-tool-calling-protocol/typescript-utcp)                | TypeScript SDK                                  | [![Stars](https://img.shields.io/github/stars/universal-tool-calling-protocol/typescript-utcp?style=social)](https://github.com/universal-tool-calling-protocol/typescript-utcp/)                |
| [`go-utcp`](https://github.com/universal-tool-calling-protocol/go-utcp)                                | Go SDK                                          | [![Stars](https://img.shields.io/github/stars/universal-tool-calling-protocol/go-utcp?style=social)](https://github.com/universal-tool-calling-protocol/go-utcp/)                                |

---

## Contributing

We welcome issues, pull requests and design discussion. **If you’d like to add support for another language, tool or framework, open a discussion first so we can align on the design!**

---

## About

UTCP is an open‑source project released under the **MPL‑2.0** license and maintained by a growing community of AI‑tooling enthusiasts. If your organization relies on direct, low‑latency access to existing API, or if you simply dislike writing wrappers, we’d love to have you involved!

---

## UTCP vs MCP

### UTCP's Core principle: 
If humans can interact with an API, AI should be able to do the same with no change in the API and the same security guarantees.

### Core Requirements
* No wrapper tax: UTCP must be able to call any tool without requiring any changes to the tool itself or the infrastructure required to call it.
* No security tax: UTCP must be able to call any tool while guaranteeing the same security as if the tool was called by a human.
* Scalable: UTCP must be able to handle a large number of tools and calls.
* Simple: UTCP must be simple to implement and use.


<p align="left">
  <img
    src="../assets/mcp-vs-utcp.gif"
    alt="UTCP vs MCP Demo"
    width="480"          
  />
</p>
