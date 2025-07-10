# Universal Tool Calling Protocol (UTCP)

<p align="center">
  <img src="assets/banner.png" alt="UTCP Logo" />
</p>

<p align="center">
  <strong>A protocol that lets AI agents call any tool, over any channel—directly and without wrappers</strong>
</p>


The **Universal Tool Calling Protocol (UTCP)** is an open standard that describes *how* to call existing tools rather than *proxying* those calls through a new server. After discovery, the agent speaks directly to the tool’s native endpoint (HTTP, gRPC, WebSocket, CLI, …), eliminating the “wrapper tax,” reducing latency, and letting you keep your existing auth, billing and security in place.

---

## Getting Started

- 📚 **Read the [Documentation](https://utcp.io)** for tutorials, examples and best practices    
- 💻 **Start building with our SDKs:**
  - [TypeScript SDK](https://github.com/universal-tool-calling-protocol/typescript-utcp)
  - [Python SDK](https://github.com/universal-tool-calling-protocol/python-utcp)

---

## Project Structure

| Repository | Description |
|------------|-------------|
| [`utcp-specification`](https://github.com/universal-tool-calling-protocol/utcp-specification) | Formal spec and reference docs |
| [`typescript-utcp`](https://github.com/universal-tool-calling-protocol/typescript-utcp) | TypeScript implementation |
| [`python-utcp`](https://github.com/universal-tool-calling-protocol/python-utcp) | Python implementation |

---

## Contributing

We welcome issues, pull requests and design discussion. 

---

## About

UTCP is an open‑source project released under the **MPL‑2.0** license and maintained by a growing community of AI‑tooling enthusiasts. If your organization relies on direct, low‑latency access to existing APIs—or if you simply dislike writing wrappers—we’d love to have you involved!
