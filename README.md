# Publish React Component
Boilerplate for publishing react component to npm

## Prerequisites
- [NodeJS (Recomendation : Latest LTS Version: v6.11.3 (includes npm 3.10.10))](https://nodejs.org/en/download/)
- [Yarn (optional, )]()

## Instalation

Just clone this repo and start developing your custom, testable react component

```
git clone https://github.com/damaera/publish-react-component &&
cd publish-react-component
```
Install npm dependencies
```
yarn install
```

## Getting Started

### React Components

* **Adding New Component**

  All React Components are in `src` directory.Components can use ES6 or ES5 standardization. 

### React Storybook
* **About**

  Reference : [ReactStoryBook](https://storybook.js.org/).

  Storybook is a UI development environment for your UI components. With it, you can visualize different states of your UI components and develop them interactively.

  Storybook runs outside of your app. So you can develop UI components in isolation without worrying about app specific dependencies and requirements.

* **Adding New Stories**

  Add new file at `stories` directory, for example can be seen on `/stories/test.stories.js`. The file must match the following format `<name>.stories.js`.

* **Adding Custom Head Tags (css/js/etc)**

  Reference : [ReactStoryBook](https://storybook.js.org/configurations/add-custom-head-tags/)

  Adding new file Simply create a file called `preview-head.html` inside the Storybook config directory `.storybook`.

* *Example*
  -	Structure
    ```
    project
    └─── .storybook
      └─── addons.js
      └─── config.js
      └─── preview-head.html
    ```
  - Inside `preview-head.html`
    ```
    <link href="https://link.com/style.css" />
    <srcipt src="https://link.com/app.js"></script>
    <script></script>
    ```

* **Adding Local Resource**

  For example, Place the `style.css` into the directory `.storybook`, and next import `./style.css` from the file `./storybook/config.js`.
  ```
  import './style.css'
  ```

* **Start StoryBook**
  ```
  yarn start
  ```

### Testing

We are using [Airbnb/Enzyme](airbnb.io/enzyme/docs/api/) with [Mocha](https://mochajs.org/) as testing utility for React that makes it easier to assert, manipulate, and traverse your React Components' output.

* **Sample**

  Please open `src/__test__/Test.js`

* **Adding New Testing**

  Place your tests file in the directory `__test__`.

* **Start Testing**
  ```
  yarn test
  ```
  or
  ```
  yarn test:watch
  ```

## Changelog
Please visit the folowing file [CHANGELOG.md](./CHANGELOG.md)

## Thins to Learn
- [ReactJS](https://facebook.github.io/react/)
- [ReactStoryBook](https://storybook.js.org/)
- [Mocha](https://mochajs.org/)
- [Airbnb/Enzyme](airbnb.io/enzyme/docs/api/)

