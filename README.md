# @gridsome/source-strapi

> [Strapi](https://strapi.io/) source for Gridsome, forked to improve functionality

## Install



## Usage

```js
module.exports = {
    siteName: "Tyler Grow",

    plugins: [
        {
            use: "@gridsome/source-strapi",
            options: {
                apiURL: "http://localhost:1337/api",
                contentTypes: ["projects"],
                qso: {
                    _limit: 1000,
                    sort: ['endDate:asc'],
                    populate: '*',
                },

            },
        },
    ],
};

```
