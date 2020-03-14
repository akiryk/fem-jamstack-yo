# Jamstack course

Create a serverless site using Netlify and Gatsby.

## Initial Setup Explained

- `yarn global add netlify-cli` so we can use command line to setup and run netlify projects. See [netlify-cli docs](https://docs.netlify.com/cli/get-started/) for all the stuff you can do with it.
- Add an empty `gatsby-config` file to let netlify know that it should use Gatsby
- Add a `netlify.toml` file for handling redirects
- Consider using [hub git tool](https://hub.github.com/)

### Enable Auth

- Use Netlify's identity tools, which is one of many ways to implement OAuth2.
- `react-netlify-identity-widget` and `react-netlify-identity` plus a couple others used behind the scenes, such as `@reach/tabs`
- Run site with Netlify, below, and enable identity on Netlify admin tools

### Run site with Netlify

- Push site to github
- Run `netlify init` in terminal
- Give yarn build command from your package file (make sure you have one there), e.g. `yarn build`
- Directory to deploy: `public`
- Run `netlify open`
- Go to settings, choose Identity, click Enable.
- Visit your Netlify site url
- Profit!

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

End.
