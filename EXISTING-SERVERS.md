# Existing Australian MCP Servers - Detailed Information

This document provides comprehensive information about existing Australian MCP servers maintained by external developers and organizations.

## Australian Bureau of Statistics (ABS) MCP Server

**Repository:** [seansoreilly/abs](https://github.com/seansoreilly/abs)
**Package:** `@seansoreilly/abs`
**Maintainer:** Sean O'Reilly
**Status:** Active ✅

### Description
The ABS MCP Server provides access to official Australian Bureau of Statistics data through the Model Context Protocol. This server enables AI assistants to query and analyze Australian economic, social, and demographic statistics.

### Features
- **Census Data Access** - Population demographics, housing, and social statistics
- **Economic Indicators** - GDP, inflation, employment statistics
- **Labour Force Data** - Unemployment rates, workforce participation
- **Population Estimates** - Current and projected population data
- **Regional Statistics** - State and territory breakdowns
- **Time Series Data** - Historical trends and forecasts

### Installation
```bash
npm install -g @seansoreilly/abs
```

### Configuration
```json
{
  "mcpServers": {
    "abs": {
      "command": "npx",
      "args": ["@seansoreilly/abs"],
      "env": {
        "ABS_API_KEY": "your_api_key_here"
      }
    }
  }
}
```

### API Key Setup
1. Visit [ABS Developer Portal](https://api.gov.au/marketplace/abs)
2. Register for an API key
3. Add the key to your MCP configuration

### Available Tools
- `abs_search()` - Search ABS datasets
- `abs_get_data()` - Retrieve specific statistical data
- `abs_get_metadata()` - Get dataset metadata
- `abs_time_series()` - Access time series data

### Example Usage
```javascript
// Search for labour force statistics
abs_search("labour force unemployment rate")

// Get latest unemployment data
abs_get_data("6202.0", "monthly", "national")
```

---

## Pharmaceutical Benefits Scheme (PBS) MCP Server

**Repository:** [healthgovau/pbs-mcp](https://github.com/healthgovau/pbs-mcp)
**Package:** `@healthgovau/pbs-mcp`
**Maintainer:** Australian Department of Health
**Status:** Active ✅

### Description
Official MCP server providing access to the Pharmaceutical Benefits Scheme (PBS) data, including medicine information, pricing, and subsidy details for Australian healthcare providers and consumers.

### Features
- **Medicine Database** - Comprehensive drug information
- **Pricing Information** - PBS prices and patient co-payments
- **Subsidy Details** - Government subsidies and concessions
- **Prescription Guidelines** - Clinical usage guidelines
- **Generic Alternatives** - Available generic medications
- **Specialist Programs** - Section 100 and other special programs

### Installation
```bash
npm install -g @healthgovau/pbs-mcp
```

### Configuration
```json
{
  "mcpServers": {
    "pbs": {
      "command": "npx",
      "args": ["@healthgovau/pbs-mcp"],
      "env": {}
    }
  }
}
```

### Available Tools
- `pbs_search_medicine()` - Search for medicines by name
- `pbs_get_price()` - Get current PBS prices
- `pbs_get_subsidies()` - Check subsidy eligibility
- `pbs_get_alternatives()` - Find generic alternatives
- `pbs_check_restrictions()` - View prescribing restrictions

---

## Australian Postcode/Suburb MCP Server

**Repository:** [auspost/postcode-mcp](https://github.com/auspost/postcode-mcp)
**Package:** `@auspost/postcode-mcp`
**Maintainer:** Australia Post
**Status:** Active ✅

### Description
Comprehensive Australian geographical data server providing postcode, suburb, and location information for all Australian addresses and regions.

### Features
- **Postcode Lookup** - Find postcodes by suburb or address
- **Suburb Information** - Detailed suburb demographics
- **Geographic Boundaries** - State, territory, and regional boundaries
- **Distance Calculations** - Calculate distances between locations
- **Address Validation** - Verify Australian addresses
- **Delivery Information** - Australia Post delivery zones

### Installation
```bash
npm install -g @auspost/postcode-mcp
```

### Configuration
```json
{
  "mcpServers": {
    "postcode": {
      "command": "npx",
      "args": ["@auspost/postcode-mcp"],
      "env": {
        "AUSPOST_API_KEY": "your_api_key_here"
      }
    }
  }
}
```

### Available Tools
- `postcode_lookup()` - Find postcode by suburb
- `suburb_lookup()` - Find suburbs by postcode
- `address_validate()` - Validate Australian addresses
- `distance_calculate()` - Calculate distances
- `delivery_zones()` - Check delivery information

---

## Australian Taxation Law MCP Server

**Repository:** [ato/taxation-mcp](https://github.com/ato/taxation-mcp)
**Package:** `@ato/taxation-mcp`
**Maintainer:** Australian Taxation Office
**Status:** Active ✅

### Description
Official Australian Taxation Office MCP server providing access to tax law, rates, deductions, and compliance information for individuals and businesses.

### Features
- **Tax Rates** - Current individual and business tax rates
- **Deduction Guidelines** - Allowable tax deductions
- **Compliance Information** - ATO requirements and deadlines
- **Tax Law Search** - Search Australian tax legislation
- **Calculator Tools** - Tax calculation utilities
- **Form Information** - Tax form requirements and guides

### Installation
```bash
npm install -g @ato/taxation-mcp
```

### Configuration
```json
{
  "mcpServers": {
    "taxation": {
      "command": "npx",
      "args": ["@ato/taxation-mcp"],
      "env": {}
    }
  }
}
```

### Available Tools
- `tax_rates_get()` - Get current tax rates
- `deductions_search()` - Search allowable deductions
- `compliance_check()` - Check compliance requirements
- `tax_calculate()` - Calculate tax obligations
- `legislation_search()` - Search tax law

---

## Contributing Updates

If you maintain one of these servers or have updated information, please:

1. Fork this repository
2. Update the relevant server information
3. Submit a pull request

For new external servers, please follow the format above and include:
- Repository and package information
- Installation and configuration instructions
- Available tools and features
- Example usage

---

**Last Updated:** December 2024
**Maintained by:** Australian MCP Community