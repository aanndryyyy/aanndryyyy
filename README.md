# Hi, I'm Andry 👋

Freelance developer from Estonia, building with Laravel, PHP and TypeScript. Lately: MCP servers for AI agents and tools for Estonian e-services.

🌐 [pedak.me](https://pedak.me) · 🏢 [arbictus.eu](https://arbictus.eu) · [@arbictus](https://github.com/arbictus)

## 🤖 MCP servers

[Model Context Protocol](https://modelcontextprotocol.io) servers that let Claude and other AI clients work with real services.

| Project | What it's for |
| --- | --- |
| [**zone-mcp**](https://github.com/aanndryyyy/zone-mcp) | Manage [Zone.ee](https://www.zone.ee) hosting from your AI client: domains, DNS records, mail forwarders, webhosting, SSL, cron, and Apache/PHP/PM2 logs over SSH. A spec-aware request tool covers the rest of the ZoneID API v2. |
| [**ariregister-mcp**](https://github.com/aanndryyyy/ariregister-mcp) | Look up Estonian companies in the e-Business Register ([Äriregister](https://ariregister.rik.ee)): company data, people and representation rights, annual reports and their figures, beneficial owners, and e-invoice readiness. Read-only. |
| [**hertwill-mcp**](https://github.com/aanndryyyy/hertwill-mcp) | Work with the [Hertwill](https://hertwill.com) dropshipping catalog: search products, manage your import list, and publish products to your Shopify or WooCommerce store at a set price. |

All three use the MCP TypeScript SDK v2 and install with one line:

```bash
claude mcp add -s user zone -- npx -y github:aanndryyyy/zone-mcp
```

## 🎨 TEDI Design System for Laravel

[**tedi-design-system-livewire**](https://github.com/aanndryyyy/tedi-design-system-livewire): unofficial Blade and Livewire components for the [TEDI Design System](https://github.com/TEDI-Design-System), an Estonian public-sector design system. TEDI ships React and Angular packages; this brings the same components to Laravel, in the style of Flux, with no JS framework needed.

```blade
<tedi:button variant="primary" icon-start="add">Lisa</tedi:button>
<tedi:alert type="warning">Tähelepanu</tedi:alert>
```

## 📒 e-Arveldaja (e-Financials)

Tools for [e-Arveldaja](https://e-arveldaja.rik.ee/), the free accounting software from the Estonian Centre of Registers and Information Systems (RIK).

| Project | What it's for |
| --- | --- |
| [**e-financials-php-client**](https://github.com/aanndryyyy/e-financials-php-client) | PHP SDK for the e-Arveldaja REST API. Handles HMAC-SHA-384 request signing and returns typed responses. Includes a `ClientFake` for tests. `composer require aanndryyyy/e-financials-php-client` |
| [**arbictus-sync-for-e-arveldaja**](https://github.com/aanndryyyy/arbictus-sync-for-e-arveldaja) | WooCommerce plugin, built on the SDK. Syncs orders to e-Arveldaja in the background: clients, products, sale invoices, payments, and credit invoices for refunds. |
