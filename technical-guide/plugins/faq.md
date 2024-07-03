---
title: 5.5. FAQ
---

# FAQ

**Which Node version should I use?**<br />
Currently we are using the v22.2.0

**Should I create my plugin for dark and light themes?**<br />
It’s not obligatory but keep in mind that the containing modal will change colors automatically to match Penpot’s theme. Check the [documentation](</technical-guide/plugins/create-a-plugin/#penpot-theme-(optional)>) for an example on how to apply dark and light themes to your plugin.

**Should I always host my plugin?**<br />
By the time being any and all plugins must be hosted independently and outside the Penpot environment. Check the [documentation](/technical-guide/plugins/deployment/) for a guide on how to deploy your plugin on some deployment services like Netlify or Cloudflare.

**Is there any way to export my figma plugins to penpot?**<br />
No. The feature set of figma and penpot are not the same so it’s not compatible.

**What is the recommended size for my plugin icon?**<br />
You can make it any size since it will be automatically adjusted to 28x28 px in the plugin manager modal. Just make sure to keep it square size.

**Are there any naming conventions for the plugin name?**<br />
The name of the plugin should be short and followed by the suffix ‘-plugins’, like ‘shape-remover-plugin’.

**Which framework do you recommend for creating the plugin?**<br />
Any framework you are familiar with would be a good choice. Our examples are in vue, angular and react. Check the [documentation](/technical-guide/plugins/create-a-plugin/#step-1.-create-a-project)

**Is it necessary to use the plugin styles library?**<br />
The plugin styles library is not obligatory, although we recommend its use because it'll help you with the dark and light theming and to maintain the Penpot look-and-feel.

**Is the API ready to use the prototyping features?**<br />
Not yet, but it’s being considered for a second phase.

**Are there any security or quality criteria I should be aware of?**<br />
There are no set requirements. However, we can recommend the use of [eslint](https://typescript-eslint.io/) or [prettier](https://prettier.io/), which is what we use.

**Is it necessary to create plugins with a UI?**<br />
No, it’s completely optional, in fact, we have an example of a plugin without UI. Try the plugin using this url to install it: `https://create-palette-penpot-plugin.pages.dev/assets/manifest.json` or check the code [here](https://github.com/penpot/penpot-plugins/tree/main/apps/create-palette-plugin)

**Can I create components?**<br />
Yes, it is possible to create components using:

```js
createComponent(shapes: PenpotShape[]): PenpotLibraryComponent;
```

Check PenpotLibrary methods in the [API documentation](/technical-guide/plugins/api/#penpotlibrary)

**Is there a place where I can share my plugin?**<br />
You will be able to share your plugin with the [Penpot community](https://community.penpot.app/). In the future, we plan to create a place where we will publish the plugins we know about, but this is still something we have to define.

**My plugin works on my local machine, but I couldn’t install it on Penpot. What could be the problem?**<br />
The url you that you need to provide in the plugin manager should look [like this](/technical-guide/plugins/create-a-plugin/#step-6.-configure-the-manifest-file): `https://yourdomain.com/assents/manifest.json`

**Where can I get support if I find a bug or an unexpected behavior?**<br />
You can report a problem or request support at <a href="mailto:support@penpot.app">support@penpot.app</a>.