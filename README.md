# contentful-extension-tables
An ui-extension to add an editable table to handle tabular data as a [Contentful UI Extension](https://www.contentful.com/developers/docs/concepts/uiextensions/).

Based on https://github.com/AnalogMemory/contentful-tables

## Installation
* In the contentful web app to to `Settings > Extensions`
* Click the `Add extension`
* Choose `Install from Github`
* Paste the link to this repository's `extensions.json` file
* Confirm selection ("Save")

**Note** This extensions is targeted at the "JSON" field-type.

### Configure
Create a configuration file with your credentials for Contentful.

```sh
cp .env.example .env
```

Open `.env` in a editor of your liking and add your Contentful space ID, and management token. [Learn how to obtain a token](https://www.contentful.com/developers/docs/references/authentication/#getting-an-oauth-token).

Load environment variables

```sh
source .env
```

### Create
```sh
npm run setup
```

Create task will register the extension in your space on Contentful.

### Update
```sh
npm run update
```

Update task will upload the extension to your space on Contentful.

## License
Copyright &copy; Contentful Developer Relations

Licensed under the [MIT license](https://github.com/contentful-labs/ui-editable-table/blob/master/LICENSE).
