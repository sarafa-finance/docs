# Sarafa Business API documentation

Merchant integration documentation for `https://api.sarafa.site/v3`, built with Mintlify.

- `docs.json` defines site navigation and appearance. `mint.json` retains matching navigation for legacy tooling.
- `api-reference/openapi.json` is the API specification. Endpoint pages explicitly reference this file.
- `api-reference/introduction.mdx` covers authentication and request conventions.
- `services/api.mdx` covers callback verification, errors, and retries.
- `services/checkout.mdx` covers hosted checkout creation and status reads.

## Preview and validate

Use the [Mintlify CLI](https://www.mintlify.com/docs/cli/install) from this directory:

```sh
npm install -g mint
mint dev
```

Before publishing:

```sh
mint validate
mint broken-links
```

Keep endpoint paths, request fields, examples, and callback signing aligned with the Sarafa Business API implementation in `sarafa/sarafabusiness/main/api` and its shared payment handlers. No credentials belong in these docs.
