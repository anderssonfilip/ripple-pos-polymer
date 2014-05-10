# Ripple Point-of-Sale

> A Web Component for Ripple (https://ripple.com/) Point of Sale. 
> Set receiving address and currency in element attributes to display QR code on your page which when
scanned will direct to a payment page.

## Demo

[Check it live!](http://tradespoke.github.io/ripple-pos-polymer/)

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install ripple-qr-pos --save
```

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="bower_components/platform/platform.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="bower_components/ripple-qr-pos/dist/ripple-qr-pos.html">
    ```

3. Start using it!

    ```html
    <ripple-qr-pos receiver="rippleaddress" currency="USD"></ripple-qr-pos>
    ```

## Options

Attribute            | Options          | Default        | Description
---                  | ---              | ---            | ---
`rippleaddress`      | *string*         | ``             | Receiving Ripple address
`currency`           | *string*         | ``             | Three character ticker
`size`               | *string/number*  | ``             | Width/height of QR box


## Development

In order to run it locally you'll need to fetch some dependencies and a basic server setup.

1. Install [Bower](http://bower.io/) & [Grunt](http://gruntjs.com/):

    ```sh
    $ [sudo] npm install -g bower grunt-cli
    ```

2. Install local dependencies:

    ```sh
    $ bower install && npm install
    ```

3. To test your project, start the development server and open `http://localhost:8000`.

    ```sh
    $ grunt server
    ```

4. To build the distribution files before releasing a new version.

    ```sh
    $ grunt build
    ```

5. To provide a live demo, send everything to `gh-pages` branch.

    ```sh
    $ grunt deploy
    ```

## License

[MIT License]
