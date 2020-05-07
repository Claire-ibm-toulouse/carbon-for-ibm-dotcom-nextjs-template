<h1 align="center"> IBM.com Library React with Next.js Template</h1>

This is a Next.js template utilizing the IBM.com Library React.

## Getting Started

This will deploy a vanilla instance of Next.js with the
[DotcomShell](https://github.com/carbon-design-system/ibm-dotcom-library/blob/master/packages/react/src/components/DotcomShell/README.md),
along with other various patterns and components available in the IBM.com Library.

To get
started:

```bash
$ yarn install
```

Then start the application:

```bash
$ yarn dev
```

To export to a static site, run the following:

```bash
$ yarn build-export
```

Then the contents of `out` can be uploaded to your production environment.

## Things to Note

If building an IBM.com page, there are items that need to be included which can be viewed here: [Building for IBM.com](https://github.com/carbon-design-system/ibm-dotcom-library/blob/master/docs/building-for-ibm-dotcom.md)

### Page Language

This template handles page language functionality, where the available languages are defined in `components/data/altlang.json`. The `Altlangs` component then generates all alternate links to be injected into the `<head>` element.

### Digital Data Object (DDO)

The Digital Data Object a flexible, customizable collection of metadata that also provides tools and services such as live chat and analytics to page authors. You can find more details on [Building for IBM.com](https://github.com/carbon-design-system/ibm-dotcom-library/blob/master/docs/building-for-ibm-dotcom.md).

The template has a placeholder DDO you can define located in the `pages/data/DDO.json` file. Example values shown below:

```
<script>
  digitalData = {
    page: {
        category: {
            primaryCategory: '' // e.g. SB03
        },
        pageInfo: {
            effectiveDate: '', // e.g. 2014-11-19
            expiryDate: '', // e.g. 2017-11-19
            language: '', // e.g. en-US
            publishDate: '', // e.g. 2014-11-19
            publisher: '', // e.g. IBM Corporation
            version: '', // e.g. dds.v1.0.0. NOTE: This is dynamically set by the IBM.com Library
            ibm: {
                contentDelivery: '', // e.g. ECM/Filegen
                contentProducer: '', // e.g. ECM/IConS Adopter 34 - GS83J2343G3H3ERG - 11/19/2014 05:14:02 PM
                country: '', // e.g. US
                industry: '', // e.g. B,U
                owner: '', // e.g. Some Person/City/IBM
                siteID: '', // e.g. MySiteID
                subject: '', // e.g. SW492
                type: '' // e.g CT305
            }
        }
    }
  };
</script>
```
