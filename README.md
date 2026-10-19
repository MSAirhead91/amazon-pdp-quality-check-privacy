# Privacy Policy for Amazon Tools

**Effective date:** August 13, 2026  
**Last updated:** October 19, 2026

Amazon Tools, formerly Amazon PDP Quality Check, is a Chrome extension for reviewing Amazon product content and supporting related workflows on supported Amazon store pages, Seller Central and Vendor Central. It currently includes PDP Checker, Case Exporter, A+ Filler and Copy Tool.

This policy explains what information the extension handles, why it is used, where it is stored and how you can delete it.

## Summary

Amazon Tools processes information in your browser. The extension has no developer-operated server and does not send product content, support conversations, imported spreadsheets, reports, settings or browsing information to the developer.

The extension contains no advertising, analytics or tracking services and requires no additional user account. It does not sell user data or use it for profiling, advertising, creditworthiness, lending or purposes unrelated to its user-facing features.

Local processing still involves handling user data. In particular, support cases may contain personal identifiers and private communications. Data can leave extension-controlled storage when you request a clipboard or file export, when the extension interacts with Amazon to provide its features, or when Chrome synchronizes the specific settings described below.

## Information handled and purposes

### PDP Checker

To check product pages, compare marketplaces, detect redirects and show changes between scans, the extension may process:

- supported Amazon page URLs, marketplace domains, ASINs and available product identifiers;
- product titles, highlights, bullet points, image and video information;
- variation information, parent and child ASINs, brand and manufacturer information;
- Standard A+, Premium A+ and Brand Story availability;
- original and destination URLs and ASINs involved in a redirect;
- product-content snapshots, change records, scan timestamps and marketplace-comparison results.

You can view results in a popup or page panel and copy them or download an Excel report. Marketplace switching supports 23 Amazon stores; detailed feature availability can vary by marketplace.

The extension processes relevant navigation on supported Amazon pages. It does not request access to Chrome's complete browsing-history database or maintain a general history of unrelated websites.

### Case Exporter

When you open or request an export of a supported Seller Central or Vendor Central support case, the extension reads available case information from the page. This can include:

- case ID, URL, page title, portal, marketplace, subject, status and dates;
- account or merchant details, including an email address if displayed in a supported account field;
- message senders, timestamps and message bodies;
- visible attachment names or links, where available.

Support conversations may contain names, contact details, account identifiers and other confidential information included in those messages. The extension does not automatically remove personal or confidential information from exports. It uses the information to display a preview, copy plain text or Markdown, or generate a TXT or PDF file at your request. It may read multiple pages of the selected case conversation; it does not send the conversation to the developer or an AI service.

### A+ Filler

When you import an Excel file, the extension processes the supported table structure and values, including ASINs, short product titles, comparison metrics and values, and supported optional fields or image references. It also stores the imported file's name.

The most recently imported table is saved locally so you can preview it and reuse it. At your request, the extension transfers supported values into an open Standard or Premium A+ comparison module in Seller Central or Vendor Central. This makes the values available to the Amazon editor under your existing Amazon session. Images are not uploaded automatically, and final review, saving and publishing remain under your control in Amazon.

You can also generate an XLSX template locally without granting Central access.

### Copy Tool

When you select text and request a Copy Tool action on a supported Central page, the extension processes the selected content to extract ASINs or EANs and generate product links. It can copy deduplicated identifiers, marketplace-specific links or a link table for your selected countries.

### Settings

The extension stores preferences such as selected marketplaces, panel behavior, notification preferences and introduction hints to provide the configured interface and features.

For Chrome Web Store disclosure purposes, these functions handle website content and web history relating to supported pages. Case Exporter also handles personally identifiable information and personal communications when these are present in a case. These disclosures apply even when processing stays on your device.

## Amazon connections and existing sessions

When you request a marketplace comparison, the extension sends direct HTTPS requests from your browser to the selected Amazon stores for the ASIN being checked. These background comparison requests omit browser credentials. Comparison starts when you expand the comparison feature.

Marketplace switching opens the relevant Amazon product or search page. Central tools interact with the supported pages you have opened using your existing signed-in Amazon session. Amazon receives information necessary for those page requests and editor interactions, subject to Amazon's own privacy policy and terms.

The extension does not ask you to provide Amazon passwords, does not read authentication cookies through Chrome's cookies API and does not transmit your login credentials to the developer.

## Storage, retention and deletion

- **Local extension storage:** Settings, introduction hints, PDP check snapshots and change history, and the latest imported A+ table and file name are stored using Chrome's extension storage APIs.
- **PDP history:** History records are treated as expired after 50 days based on the stored current-snapshot timestamp. Expired records are removed during the extension's history cleanup or replaced when a new scan is recorded. This is not a guarantee of deletion at an exact wall-clock time.
- **A+ table:** The latest imported table remains locally available until you replace or delete it, clear the saved tool data, or remove the extension's local data.
- **Session storage:** Marketplace-comparison results and temporary navigation or redirect information are held in Chrome's session storage. Comparison results are reused for up to 30 minutes before being refreshed; the cache lifetime is not a promise that each entry is physically deleted after exactly 30 minutes.
- **Case and copy processing:** Case previews and selected-text extraction are used for the current operation. The extension does not maintain a persistent support-case archive in its local extension storage.
- **Chrome Sync:** Selected marketplaces and the setting to open the PDP panel automatically after a country switch use Chrome Sync. Depending on your Chrome settings, Google may synchronize these preferences across your signed-in browsers. PDP check histories, imported A+ tables and support conversations are not placed in Chrome Sync by the extension.

You can delete the saved A+ table and all PDP check histories from the general settings. The table can also be removed in A+ Filler, and PDP histories can be deleted through the available history controls. Clearing saved tool data preserves your country selection and other preferences.

Deleting extension-stored data does not delete the original Excel files, exported files or clipboard contents on your computer. Those remain under your control. Removing the extension removes extension-controlled local data according to Chrome's behavior; synchronized preferences are subject to Chrome's synchronization and data-management controls.

## Clipboard and exported files

Amazon Tools writes to the clipboard only following a copy action. It does not read clipboard contents.

TXT, PDF and XLSX files are generated in your browser and saved when you request the corresponding export or template. There is no developer-operated conversion service. The extension does not upload these files to the developer.

You control subsequent use, storage and sharing of copied or exported information. Other software or services you choose to use with that information operate under their own data practices.

## Permissions

Amazon Tools uses the following required permissions for its visible functions:

- **activeTab:** user-initiated interaction with the supported page in the active tab.
- **scripting:** injecting bundled code and styles to read supported pages, display the panel and perform authorized tool actions.
- **storage:** local settings and saved tool data, temporary session data and the limited Chrome Sync preferences described above.
- **contextMenus:** commands for PDP checks, marketplace switching, case exports, reuse of an A+ table and copying identifiers or links.
- **clipboardWrite:** copying information following a user action.
- **webNavigation:** associating supported Amazon product-page navigation and ASIN redirects, and opening the panel after a marketplace switch when enabled.
- **notifications:** optional desktop alerts about detected ASIN redirects, containing source and destination ASINs. You can disable these alerts in settings.
- **Amazon store host permissions:** accessing the 23 supported HTTPS Amazon store domains listed in the extension manifest for PDP checks, panel display and requested marketplace comparisons.

Additional permissions are optional and requested when needed:

- **Seller Central and Vendor Central host access:** requested for the domain being used to read a support case, process selected content or fill an open A+ comparison module.
- **downloads:** requested for user-initiated TXT/PDF case exports through Chrome's downloads API. The extension does not use this permission to analyze your download history. Excel templates and PDP Excel reports use normal file downloads without this optional permission.

You can decline optional permissions or revoke them through Chrome. Actions that require a declined permission will not run.

## Sharing, security and restricted use

Amazon Tools does not transfer handled content to the developer, advertising networks, analytics providers or data brokers and does not sell user data. The Amazon connections, limited Google Chrome Sync preferences and user-directed clipboard/file outputs described above are used only to provide the extension's features.

Website access is restricted to the supported domains in the manifest, with additional Central access requested when needed. Amazon requests use HTTPS. JavaScript and the PDF/XLSX libraries are bundled with the extension; it does not execute remotely hosted code.

The developer has no extension-provided access to locally processed user content. The extension does not monitor general clicks, keystrokes or mouse movements for analytics or behavioral profiling.

## Chrome Web Store Limited Use disclosure

Amazon Tools uses information accessed through Chrome APIs only to provide its disclosed user-facing features. Its use and transfer of user data adhere to the Chrome Web Store User Data Policy, including the Limited Use requirements. User data is not used for personalized advertising, unrelated profiling, creditworthiness or lending.

## Changes to this policy

This policy may be updated when Amazon Tools' features or data practices change. Updated versions will be published at this location with a revised "Last updated" date. The repository address retains the former product name for continuity.

## Contact

Questions about this policy can be submitted through the public issue tracker:

https://github.com/MSAirhead91/amazon-pdp-quality-check-privacy/issues

Issues are public. Do not include private support conversations, personal information, account credentials or unredacted files in an issue.

## Independent product

Amazon Tools is an independent browser extension and is not affiliated with, endorsed by or sponsored by Amazon.

