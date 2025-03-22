# SLOP MCP

A Model Context Protocol (MCP) server for Claude that enables searching and exploring OpenAPI specifications through oapis.org.

## Features

- Get an overview of any OpenAPI specification
- Retrieve details about specific API operations
- Support for both JSON and YAML formats
- Works with Claude Desktop

## Installation

```bash
npx slop-mcp init
```

## Usage in Claude

Once installed, you can ask Claude to:

- "Find information about the Stripe API"
- "Explain how to use the GitHub API's repository endpoints"
- "Get details about the Spotify API's authentication"

Claude will use the MCP server to:

1. First get an overview of the requested API
2. Then retrieve specific operation details as needed

## API Identifiers

- Use known API IDs from openapisearch.com
- Or use any URL by removing the protocol and replacing slashes with `__`
  - Example: `api.example.com__v1__users` instead of `api.example.com/v1/users`

## Requirements

- Node.js >= 16.17.0
- Claude Desktop (for full integration)

## License

MIT
