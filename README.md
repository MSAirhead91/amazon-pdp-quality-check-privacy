# Privacy Policy for Amazon PDP Quality Check

**Effective date:** August 13, 2026  
**Last updated:** August 13, 2026

Amazon PDP Quality Check is a Chrome extension for reviewing product detail pages on supported European Amazon marketplaces. This Privacy Policy explains what information the extension handles and how that information is used.

## Summary

Amazon PDP Quality Check does not transmit personal data, browsing data, product-page content, reports, analytics, or usage information to the developer or to analytics, advertising, or tracking services. The extension has no developer-operated server. Information handled by the extension remains in the user's browser, except when the browser connects directly to Amazon to load or compare a product page.

## Information handled by Amazon PDP Quality Check

To provide its user-facing features, Amazon PDP Quality Check may process:

- the URL, marketplace, and ASIN of a supported Amazon product page;
- product titles, article highlights, and bullet points;
- image and video counts;
- variations and child ASINs;
- A+ Content and Brand Story availability;
- product redirects and marketplace availability;
- product-page snapshots used to identify changes between scans; and
- extension settings and temporary marketplace-comparison results.

Because URLs and product-page elements relate to websites visited by the user, Chrome Web Store disclosures classify some of this information as web history and website content.

## How information is used

Amazon PDP Quality Check uses this information only to provide its single purpose: reviewing the completeness and consistency of Amazon product detail pages. This includes displaying a quality overview, comparing an ASIN across supported European Amazon marketplaces, detecting ASIN redirects, showing changes between scans, and copying content or reports when requested by the user.

Amazon PDP Quality Check does not use information for advertising, profiling, creditworthiness, lending, or any purpose unrelated to its user-facing features.

## Marketplace comparison requests

When the marketplace-comparison feature is used, the extension sends direct HTTPS requests from the user's browser to the supported Amazon marketplaces for the ASIN being reviewed. These requests retrieve the corresponding public product pages required for the comparison.

Requests are sent directly to Amazon and not to the developer. The extension omits browser credentials from these background requests. Amazon may process requests according to its own privacy policy and terms.

## Local storage and retention

The extension stores interface preferences, panel settings, product-page scan snapshots, and temporary operating data locally through Chrome's extension storage APIs.

Marketplace-comparison results are cached in session storage for up to 30 minutes. Product-page scan history expires after 50 days and can also be deleted for an ASIN from the extension interface. Removing the extension through Chrome removes extension-controlled local storage according to Chrome's behavior.

No locally stored extension data is synchronized with or transmitted to the developer.

## Clipboard

The extension writes product content, child ASINs, or quality reports to the clipboard only when the user selects a copy function. It does not read clipboard contents.

## Data transmission and sharing

Amazon PDP Quality Check does not send handled information to the developer, analytics providers, advertising networks, data brokers, or other third parties. It does not sell user data.

The direct HTTPS requests to Amazon described above occur solely to provide the marketplace-comparison feature. Amazon websites operate under their own privacy policies, and Amazon PDP Quality Check does not control their data practices.

## Permissions

Amazon PDP Quality Check uses Chrome permissions only to provide visible extension features:

- **Active tab:** identifies and interacts with the supported Amazon product page in the active tab after a user action.
- **Scripting:** inserts packaged extension code and styles when needed to analyze the Amazon product page and display the quality-check panel.
- **Storage:** saves interface preferences, scan snapshots, redirect information, and temporary marketplace results locally.
- **Context menus:** provides an optional right-click command for opening the quality-check panel.
- **Clipboard write:** copies content, child ASINs, and reports only when requested by the user.
- **Web navigation:** detects when Amazon redirects a requested product URL or ASIN to another ASIN.
- **Website access:** reads supported Amazon product pages and retrieves corresponding public product pages for marketplace comparisons.

## Security

Amazon PDP Quality Check minimizes data handling, limits website access to the supported European Amazon domains listed in its manifest, and uses HTTPS for marketplace requests. The extension uses packaged code and does not execute remotely hosted code.

The extension contains no advertising, analytics, tracking services, or user accounts.

## Chrome Web Store Limited Use disclosure

The use of information received from Google APIs will adhere to the Chrome Web Store User Data Policy, including the Limited Use requirements.

## Changes to this policy

This Privacy Policy may be updated when Amazon PDP Quality Check's features or data practices change. Any updated version will be published at this location with a revised “Last updated” date.

## Contact

Questions about this Privacy Policy can be submitted through the public issue tracker at:

https://github.com/MSAirhead91/amazon-pdp-quality-check-privacy/issues

## Independent product

Amazon PDP Quality Check is an independent browser extension and is not affiliated with, endorsed by, or sponsored by Amazon.

