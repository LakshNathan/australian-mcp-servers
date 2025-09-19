# Australian Industry MCP Servers - Complete Directory

A comprehensive collection of Model Context Protocol (MCP) servers for Australian businesses, government agencies, and industry-specific data sources.

## Overview

The Model Context Protocol (MCP) enables AI assistants to securely connect to data sources and tools. This repository serves as the central hub for Australian MCP servers across all industries, making it easier for developers to integrate Australian business and government data into their AI applications.

### Why Australian Industry Data Matters

Australian industry data provides:
- **Local business intelligence** - Access to Australian market data and insights
- **Industry-specific tools** - Specialized APIs for Australian sectors
- **Regulatory compliance** - Understanding Australian business regulations
- **Market context** - Local economic, demographic, and business insights
- **Corporate integration** - Direct access to Australian company services

## Quick Start

1. **Choose a server** from the industry directory below
2. **Install** the server (see installation instructions)
3. **Configure** your MCP client (Claude Desktop, VS Code, etc.)
4. **Start using** Australian industry data in your AI workflows

## Australian Industry MCP Servers Directory

### 🏛️ Government & Public Services
- **[ABS MCP Server](https://github.com/seansoreilly/mcp-server-abs)** ✅ **ACTIVE**
  - Australian Bureau of Statistics Data API access
  - **Author:** Sean O'Reilly
  - **Installation:** `git clone https://github.com/seansoreilly/mcp-server-abs.git`

- **[PBS MCP Server](https://github.com/matthewdcage/pbs-mcp-server)** ✅ **ACTIVE**
  - Pharmaceutical Benefits Scheme data and pricing
  - **Author:** Matthew Cage (AI Advantage)
  - **Installation:** `git clone https://github.com/matthewdcage/pbs-mcp-server.git`

### 💼 Recruitment & HR
*Coming Soon - Contributions Welcome!*
- SEEK Jobs API MCP Server
- Indeed Australia MCP Server
- LinkedIn Australia MCP Server
- Hays Recruitment MCP Server

### 🏢 Corporate Services
*Coming Soon - Contributions Welcome!*
- Australia Post MCP Server (tracking, postcode lookup)
- Telstra Business API MCP Server
- Xerox Australia MCP Server

### 🏦 Financial Services
*Coming Soon - Contributions Welcome!*
- Commonwealth Bank API MCP Server
- ANZ Business API MCP Server
- Westpac API MCP Server
- NAB Connect MCP Server
- Xero Accounting MCP Server
- MYOB MCP Server

### 🛒 Retail & E-commerce
*Coming Soon - Contributions Welcome!*
- Woolworths API MCP Server
- Coles API MCP Server
- Bunnings MCP Server
- JB Hi-Fi MCP Server

### 🏗️ Construction & Mining
*Coming Soon - Contributions Welcome!*
- BHP Data MCP Server
- Rio Tinto MCP Server
- Wesfarmers MCP Server
- CSL MCP Server

### 📱 Technology
*Coming Soon - Contributions Welcome!*
- Atlassian API MCP Server
- Canva API MCP Server
- SafetyCulture (iAuditor) MCP Server
- Campaign Monitor MCP Server

### ✈️ Travel & Transport
*Coming Soon - Contributions Welcome!*
- Qantas API MCP Server
- Jetstar MCP Server
- Sydney Airport MCP Server
- Uber Australia MCP Server

### 🏥 Healthcare
*Coming Soon - Contributions Welcome!*
- Medibank MCP Server
- Bupa Australia MCP Server
- Health Direct MCP Server

### 📺 Media & Telecommunications
*Coming Soon - Contributions Welcome!*
- ABC iView MCP Server
- SBS On Demand MCP Server
- Foxtel API MCP Server
- News Corp Australia MCP Server

### 🏛️ Education
*Coming Soon - Contributions Welcome!*
- Australian Universities MCP Server
- TAFE API MCP Server
- Education Australia MCP Server

## Installation Instructions

### For Claude Desktop

Add to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "abs": {
      "command": "node",
      "args": ["/path/to/mcp-server-abs/dist/index.js"],
      "env": {}
    },
    "pbs": {
      "command": "python", 
      "args": ["/path/to/pbs-mcp-server/main.py"],
      "env": {}
    },
    "seek": {
      "command": "npx",
      "args": ["australian-seek-mcp"],
      "env": {
        "SEEK_API_KEY": "your_api_key"
      }
    }
  }
}
```

## Contributing Guidelines

We welcome contributions from Australian businesses and developers!

### For Australian Companies

🏢 **Is your company Australian?** We'd love to have your MCP server in this directory!

1. **Create an MCP server** for your public APIs
2. **Submit a pull request** with your server details
3. **Get featured** in the Australian MCP ecosystem
4. **Help the community** access Australian business data

### Adding New Industry Servers

1. **Fork** this repository
2. **Choose the right industry category** from above
3. **Create** a comprehensive MCP server
4. **Include** proper documentation and examples
5. **Submit** a pull request

### Server Requirements

- Must be from an **Australian company or organization**
- Provide access to **Australian business/industry data**
- Include comprehensive setup instructions
- Follow MCP protocol standards
- Include proper API authentication
- Provide example usage

### Naming Convention

Use: `australian-[company/industry]-mcp`
- Examples: `australian-seek-mcp`, `australian-commbank-mcp`

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
```

## Resources

- [Model Context Protocol Documentation](https://modelcontextprotocol.io/)
- [Australian Government Data Portal](https://data.gov.au/)
- [Australian Business Register](https://abr.business.gov.au/)
- [ACCC Competition & Consumer Act](https://www.accc.gov.au/)

## Call to Action

### For Australian Businesses
🚀 **Make your data AI-accessible!** Create an MCP server for your APIs and join the Australian AI ecosystem.

### For Developers  
🛠️ **Build industry-specific tools!** Help connect Australian businesses to the AI revolution.

### For Contributors
🤝 **Join the community!** Help build the definitive directory of Australian industry MCP servers.

## License

This repository is licensed under the MIT License. Individual MCP servers may have their own licenses.

## Acknowledgments

**Current Contributors:**
- **Sean O'Reilly** - [ABS MCP Server](https://github.com/seansoreilly/mcp-server-abs)
- **Matthew Cage** - [PBS MCP Server](https://github.com/matthewdcage/pbs-mcp-server)

**Industry Partners:** *Seeking partnerships with Australian companies*

---

**🇦🇺 Proudly Australian** | **Maintained by the Australian MCP Community** | **Last Updated:** December 2024
