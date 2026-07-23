# POE BOTTARI Trade Privacy Policy

Effective date: July 23, 2026

This policy describes how the **POE BOTTARI Trade** Chrome extension handles data. The extension is a local browser companion for Path of Exile build, economy, and trade workflows.

## Data handled by the extension

### Supported-site translation

Site translation is off by default. When the user enables a supported site and grants that site's optional permission, the extension reads visible page text needed for translation and replaces matching interface and game terms in the page. Translation uses data packaged with the extension and runs on the user's device.

The extension stores the selected translation language and per-site on/off settings in `chrome.storage.local`.

### Trade actions

On supported Path of Exile trade pages, the extension adds explicit PoB action buttons. Only when the user clicks one of these buttons, the extension handles:

- the selected trade item's text;
- the current trade-page URL;
- the selected action and PoE game identifier.

This data is sent through Chrome Native Messaging only to the POE BOTTARI application installed on the same computer. It is used to add the selected item to the managed Path of Building runtime or calculate the item's local PoB effect.

When an item does not already expose its clipboard text in the page, the extension may request the item's JSON representation from the same official Path of Exile trade origin. That request omits browser credentials.

## Data not collected

The developer does not receive or retain the page text, trade item text, trade URL, translation settings, or PoB action data handled by the extension.

The extension does not:

- use analytics, advertising, tracking pixels, or behavioral profiling;
- sell or transfer user data;
- read or store browser cookies, POESESSID values, passwords, OAuth tokens, payment information, or browser history;
- send page content to an external translation service;
- allow the developer or another human to read data handled locally by the extension.

## Permission purposes

- `nativeMessaging`: connect to the locally installed POE BOTTARI application.
- `scripting`: register and run the packaged local translation scripts only on sites the user enables.
- `storage`: save the selected language and per-site translation settings on the user's device.
- Path of Exile trade-page access: add explicit PoB controls and process the selected item when the user invokes an action.
- Optional site access: translate visible page text only after the user enables and grants access to that exact supported site.

## Sharing and third parties

The extension does not send handled user data to the developer, advertising networks, data brokers, or analytics providers. Normal browser requests remain subject to the privacy practices of the website the user is visiting. The same-origin official trade-item request described above is made only to provide the user-requested trade action.

## Retention and deletion

The developer has no server-side copy of extension data to retain or delete. Users can turn off individual sites in the extension popup, remove a site's permission in Chrome, clear the extension's local storage, or uninstall the extension.

## Chrome Web Store Limited Use

The use of information received from Chrome APIs adheres to the [Chrome Web Store User Data Policy](https://developer.chrome.com/docs/webstore/program-policies/user-data-faq), including the Limited Use requirements. Data is handled only to provide the extension's disclosed user-facing features.

## Changes

If the extension's data practices change, this policy and the in-product disclosure will be updated before the changed handling is introduced.

## Contact

For privacy or support questions, open an issue in the [POE BOTTARI Releases repository](https://github.com/Hansihoo/POE-BOTTARI-Releases/issues). Do not post credentials, private build data, or other secrets.
