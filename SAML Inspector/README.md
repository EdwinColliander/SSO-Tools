# SAML Inspector

A lightweight, browser-based tool for inspecting and troubleshooting SAML 2.0 federations. Built as a single HTML file — no installation, no dependencies, no data leaving your machine.

## Features

- Parse and inspect SP/IdP metadata, including certificate details (CN, SAN, expiry)
- Parse AuthnRequest messages (XML or Base64)
- Parse SAML Responses and Assertions with automatic XML signature verification using the embedded certificate
- Decode/encode SAMLRequest and SAMLResponse for both Redirect Binding (DEFLATE + Base64) and POST Binding (Base64)
- Inspect X.509 certificates — subject, issuer, SAN, validity, fingerprints (SHA-1 / SHA-256)

## Usage

Download `saml-inspector.html` and open it in any modern browser. An internet connection is required on first load to fetch [pako](https://github.com/nodeca/pako) (DEFLATE) and [forge](https://github.com/digitalbazaar/forge) (crypto). After that it works fully offline.

> No data is transmitted anywhere. All processing happens locally in the browser.

## License

Free to use for any purpose. This tool is provided as-is, without warranty of any kind. The author takes no responsibility for any issues, damages or security implications arising from its use. Use at your own risk.
