# Jamstack course

Create a serverless site using Netlify and Gatsby.

## Initial Setup

- `yarn global add netlify-cli` so we can use command line to setup and run netlify projects. See [netlify-cli docs](https://docs.netlify.com/cli/get-started/) for all the stuff you can do with it.
- Add an empty `gatsby-config` file to let netlify know that it should use Gatsby
- Add a `netlify.toml` file for handling redirects

### Auth

- Use Netlify's identity tools, which is one of many ways to implement OAuth2.
- `react-netlify-identity-widget` and `react-netlify-identity`.

### Prettier

- Use Prettier Code Formatter extension in VSCode
- Add `"editor.formatOnSave": true` to VSCode user settings

```json
{
  "trailingComma": "es5",
  "tabWidth": 2,
  "semi": true,
  "singleQuote": true
}
```
