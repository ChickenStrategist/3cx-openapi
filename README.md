# 3CX Configuration API (XAPI) - Starter OpenAPI

Official OpenAPI 3.0 specification for 3cx API integration with Rewst.

## Documentation
[Rewst Custom Integration Guide](https://docs.rewst.help/documentation/configuration/integrations/custom-integrations/custom-integrations-v2)

## Specification Details
- **Version**: v20-starter-1.0.0
- **Base URL**: `https://{pbxFqdn}`
- **Authentication**: BearerAuth

## Description
Starter OpenAPI specification for integrating with the 3CX Configuration API (XAPI) introduced in 3CX v20.
This file covers the client credentials token flow and a representative subset of configuration endpoints.
**Note:** 3CX's XAPI is OData-based; many collections support `$filter`, `$select`, `$top`, etc.
Extend this spec with additional entities (Queues, Trunks, System Extensions, Routing, etc.) as needed.


## Usage

### Import into Rewst
1. Navigate to: Rewst Dashboard > Configuration > Integrations
2. Create Custom Integration
3. Upload `openapi.json` from this repository
4. Configure authentication parameters
5. Test connection

### Import into API Testing Tools
- **Postman**: Import > Link > Paste raw GitHub URL
- **Insomnia**: Import > URL > Paste raw GitHub URL
- **OpenAPI Generator**: `openapi-generator-cli generate -i openapi.json`

## Repository Structure
```
.
├── openapi.json              # Primary OpenAPI 3.0 specification
├── assets/                   # Integration assets (logos, guides)
├── README.md                 # This file
└── .github/
    └── workflows/
        └── validate-openapi.yml  # CI validation
```

## Validation
This specification is automatically validated on every commit using GitHub Actions.

## Contributing
Maintained by Rewst APAC Automation Team.

## Support
- **Technical Support**: roc@rewst.io
- **Documentation**: [Rewst Docs](https://docs.rewst.help)

## License
Private repository - Rewst LLC internal use only.
