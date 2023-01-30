# io-app-email-templates

This repo contains the mail template(s) sent on behalf of IO App and its services. Templates are created using [MJML](https://mjml.io/) markup language.

## How to apply changes

To edit them, you can choose among these following options:

- [Online editor](https://mjml.io/try-it-live)
- [Local installation](https://mjml.io/download)
- [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=mjmlio.vscode-mjml)

To generate the HTML output you need to run the generate script

```shell
$ yarn generate
```

## How to deploy changes

### MailValidation
1. Release a new tag from main branch containing the new template version.
2. Clone the project https://github.com/pagopa/io-functions-app
3. In the package.json, update the generate:templates:mailvalidation url to point to the tag relesed at (1)
4. Push, PR and merge the changes to io-funcions-app
5. Release the new version of io-functions-app 

## Compatibility

Templates are compatible with the following clients:

- Apple Mail 13+ (dark mode included)
- Gmail Web app
- OL Office 365 (dark mode included, partially supported on Windows)
- Outlook 2013, 2016, 2019, 2021 (dark mode included, partially supported on Windows)
- Windows 10 Mail (dark mode partially supported)
- Windows 11 Mail
- Gmail App (Android 6+, dark mode partially supported)
- Gmail App (iOS 13.1+, dark mode partially supported)
- iPad (iOS 13.1+)
- iPhone (iOS 13.1+)
- AOL Mail
- Outlook.com Mail (dark mode partially supported)
- Yahoo! Mail

### Related mail templates

- [Area Riservata (former SelfCare)](https://github.com/pagopa/selfcare-email-templates)
- [Piattaforma Notifiche](https://github.com/pagopa/pn-email-templates)
- [pagoPA](https://github.com/pagopa/pagopa-email-templates)
