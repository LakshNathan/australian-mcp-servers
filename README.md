# Australian Government MCP Servers - Complete Directory

A comprehensive collection of Model Context Protocol (MCP) servers providing access to Australian Government data, statistics, and services.

## Overview

The Model Context Protocol (MCP) enables AI assistants to securely connect to data sources and tools. This repository serves as the central hub for Australian Government MCP servers, making it easier for developers to integrate Australian data into their AI applications.

### Why Australian Government Data Matters

Australian Government data is crucial for:
- **Evidence-based decision making** - Access to official statistics and datasets
- **Compliance and regulations** - Understanding Australian laws, taxation, and healthcare systems
- **Local context** - Geographical, demographic, and economic insights specific to Australia
- **Public services** - Integration with government services and APIs

## Quick Start

1. **Choose a server** from the directory below
2. **Install** the server: `npm install -g [package-name]`
3. **Configure** your MCP client (Claude Desktop, VS Code, etc.)
4. **Start using** Australian Government data in your AI workflows

## Complete Directory of Australian MCP Servers

### Statistics & Data
- **[ABS (Australian Bureau of Statistics)](https://github.com/seansoreilly/abs)** - `@seansoreilly/abs`
  - Official Australian economic, social, and population statistics
  - Census data, labour force statistics, population estimates
  - Installation: `npm install -g @seansoreilly/abs`

### Healthcare & Pharmaceuticals
- **[PBS API (Pharmaceutical Benefits Scheme)](https://github.com/healthgovau/pbs-mcp)** - `@healthgovau/pbs-mcp`
  - Pharmaceutical Benefits Scheme data and pricing
  - Medicine information and subsidies
  - Installation: `npm install -g @healthgovau/pbs-mcp`

### Geography & Location
- **[Australian Postcode/Suburb Server](https://github.com/auspost/postcode-mcp)** - `@auspost/postcode-mcp`
  - Comprehensive Australian postcode and suburb data
  - Geographic boundaries and location services
  - Installation: `npm install -g @auspost/postcode-mcp`

### Legal & Taxation
- **[Australian Taxation Law Server](https://github.com/ato/taxation-mcp)** - `@ato/taxation-mcp`
  - Australian taxation law and regulations
  - Tax rates, deductions, and compliance information
  - Installation: `npm install -g @ato/taxation-mcp`

## Servers in This Repository

*This section will contain servers developed and maintained within this repository.*

Coming soon:
- Australian Business Register (ABR) MCP Server
- ASIC Company Information MCP Server
- Weather Bureau Data MCP Server
- Education Statistics MCP Server

## Installation Instructions

### For Claude Desktop

Add to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "abs": {
      "command": "npx",
      "args": ["@seansoreilly/abs"],
      "env": {
        "ABS_API_KEY": "your_api_key_here"
      }
    },
    "pbs": {
      "command": "npx",
      "args": ["@healthgovau/pbs-mcp"],
      "env": {}
    }
  }
}
```

### For VS Code

Add to your MCP configuration:

```json
{
  "servers": {
    "abs": {
      "command": "npx",
      "args": ["@seansoreilly/abs"]
    }
  }
}
```

## Contributing Guidelines

We welcome contributions to expand the Australian MCP ecosystem!

### Adding New Servers

1. **Fork** this repository
2. **Create** a new directory under `servers/` for your server
3. **Include** comprehensive documentation
4. **Follow** our naming convention: `australian-[department/agency]-mcp`
5. **Submit** a pull request with your server

### Server Requirements

- Must provide access to official Australian Government data
- Include comprehensive README with setup instructions
- Follow MCP protocol standards
- Include proper error handling and logging
- Provide example usage and configuration

### Updating Existing Server Info

1. Fork this repository
2. Update the relevant sections in README.md or EXISTING-SERVERS.md
3. Ensure links and installation instructions are current
4. Submit a pull request

## Development

```bash
# Clone the repository
git clone https://github.com/LakshNathan/australian-mcp-servers.git
cd australian-mcp-servers

# Install dependencies for all servers
npm install
npm run install-all

# Run tests
npm test

# Lint and format
npm run lint
npm run format
```

## Resources

- [Model Context Protocol Documentation](https://modelcontextprotocol.io/)
- [Australian Government Data Portal](https://data.gov.au/)
- [Australian Bureau of Statistics](https://www.abs.gov.au/)
- [Department of Health](https://www.health.gov.au/)

## License

This repository is licensed under the MIT License. Individual MCP servers may have their own licenses - please check each server's repository.

## Acknowledgments

Special thanks to the Australian Government departments and agencies making their data accessible, and to the developers creating MCP servers for the Australian ecosystem.

---

**Maintained by the Australian MCP Community** | **Last Updated:** December 2024