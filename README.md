# Mintlify Aegister S.p.A.

### Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify) to preview the documentation changes locally. To install, use the following command

```
npm i -g mintlify
```

Run the following command at the root of your documentation (where mint.json is)

```
mintlify dev
```

To automatically import the API schema run the following

```
npx @mintlify/scraping@latest openapi-file https://app.aegister.com/api/v1/schema/ -o api-reference
```

### Publishing Changes

Changes will be deployed to production automatically after pushing to the default branch.

#### Troubleshooting

- Mintlify dev isn't running - Run `mintlify install` it'll re-install dependencies.
- Page loads as a 404 - Make sure you are running in a folder with `mint.json`
