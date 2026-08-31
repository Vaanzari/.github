# Vaanzari

Vaanzari is a Banarasi saree marketplace focused on public catalogue discovery,
artisan context, and agent-assisted shopping.

## Explore Vaanzari

- [Visit the storefront](https://vaanzari.com)
- [Read the public MCP + WebMCP repository](https://github.com/Vaanzari/vaanzari-commerce-mcp)

## Services and agent integrations

### Remote MCP

Connect a compatible MCP client to [`https://vaanzari.com/mcp`](https://vaanzari.com/mcp)
over Streamable HTTP. Public catalogue and artisan discovery are available
without OAuth. Customer-scoped actions, when supported by a client, require
the user's explicit authorization.

### Browser WebMCP

The public [`vaanzari-commerce-mcp`](https://github.com/Vaanzari/vaanzari-commerce-mcp)
repository contains a standalone browser-native WebMCP reference implementation.
When supported by the browser, it registers these page-native tools through
`document.modelContext.registerTool(...)`:

- `search-sarees` — search the public catalogue
- `get-saree` — inspect a public saree listing
- `compare-sarees` — compare available listings
- `open-saree` — open a listing in the storefront
- `add-saree-to-cart` — add an available listing to the visible cart
- `open-cart` — open the visible cart

WebMCP stops at visible cart state. Checkout, payment, account, order, and
other sensitive actions remain human-controlled. Native WebMCP support depends
on the browser; a browser fallback is not native tool-registration proof.

## Build with the public reference

Start with the [MCP/WebMCP quickstart](https://github.com/Vaanzari/vaanzari-commerce-mcp/blob/main/docs/quickstart.md),
[tool guide](https://github.com/Vaanzari/vaanzari-commerce-mcp/blob/main/docs/tools.md),
and [browser verification guide](https://github.com/Vaanzari/vaanzari-commerce-mcp/blob/main/docs/browser-verification.md).

The public repository is independently runnable and contains public-safe
fixture data, diagnostics, examples, tests, and integration documentation. It
does not contain production credentials, customer data, payment logic, or
administrative interfaces.

## Contact

For customer, catalogue, privacy, or integration questions, use the verified
[Vaanzari contact channels](https://vaanzari.com/contact).
