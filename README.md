# EBI Template for reveal.js

This is a reconstructions of the EMBL-EBI presentation templates using the [reveal.js](https://revealjs.com/) presentation framework.

The reconstruction is not exhaustive but at least is functional in its current state.

Here is a [demo](https://gustavo-salazar.github.io/EBI-reveal.js-template/).

### How to use it

One way you can use this template is:

1. Clone this repo:
   ```sh
   git clone https://github.com/gustavo-salazar/EBI-reveal.js-template.git
   ```
2. Install the dependencies:
   ```sh
   cd EBI-reveal.js-template
   npm install
   ```
3. Run the developer's server and open a browser in http://localhost:1234

   ```sh
   npm run start
   ```

4. And edit the `src/index.html` file for your presentation.

---

#### Multiple presentations

You can create multiple presentation files in the same installation. Just make sure to include them as sources in the `package.json` file. For example:

```js
{
  //...
    "source": [
      "src/index.html",
      "src/secondPresentation.html",
    ]
  //...
}
```

Then you'll be able to see it in your browser in http://localhost:1234/secondPresentation.html

---

#### Customizing the reveal.js setup.

The loading of the reveal.js framework happens on `src/index.js`.

The general configuration can be edited there. And all the configuration option can be seen [HERE](https://revealjs.com/config/)

It currently only includes 2 of the reveal plugins: Markdown, Highlight. But you can add [other plugins](https://revealjs.com/plugins/).
