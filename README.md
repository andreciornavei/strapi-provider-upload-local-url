# strapi-provider-upload-local-url

## π &nbsp; _Overview and Motivation_

This provider reflects the `strapi-provider-upload-local`  but with an additional option to set the `baseurl` on upload url data as prefix.

Generally the provider-upload-local is used for development purposes and other providers already implements the baseurl of the provided solution, this provider just prevents refactoring when changes from development environment to staging/production environments.

---

## π» &nbsp;  _Example._

`config/plugins.js`
```js
module.exports = ({ env }) => {
  return ({
    upload: {
      provider: 'local-url',
      providerOptions: {
        baseurl: "http://localhost:1337"
      },
    },
  })
};
```

---

## π &nbsp;  _Congradulations, You're done._

I hope this plugin helps you in your strapi projects and save a lot of time and code.

---
## π &nbsp; _License_

This project is under the MIT license. See the [LICENSE](./LICENSE) for details.

--- 

π» &nbsp; Developed by AndrΓ© Ciornavei - [Get in touch!](https://www.linkedin.com/in/andreciornavei/)