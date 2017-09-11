# Resin Components

[![Build Status](https://travis-ci.org/resin-io-modules/resin-components.svg?branch=master)](https://travis-ci.org/resin-io-modules/resin-components)

A collection of resin.io UI components, built using [Preact][preact], [recompose][recompose], [styled-components][styled-components] and [styled-system][styled-system].

## Usage

You can import preact components directly into your project:

```jsx
import { h } from 'preact';
import { Button, Box } from 'resin-components';

const Example = () => {
  return (
    <Box my={3} className="example-button-wrapper">
      <Button primary emphasized>Click me</Button>
    </Box>
  )
};

export default Example;
```

### Provider

Wrap your application in the `<Provider>` component so that child components can correctly inherit the resin theme. You can optionally provide your own theme.

### Styled system

All components support [styled-system][styled-system] attributes, allowing you to use `fontSize`, `color`, `px` etc.

### UI Components

For and interactive demo of all components, see https://resin-io-modules.github.io/resin-components

## Developing

Clone this repository and then run:

```sh
npm install
```

The interactive storybook can be launched by running:

```sh
npm run storybook
```

Code is automatically linted and formatted by [Husky][husky] as a pre-commit hook.

The interactive storybook can be published by running:

```sh
npm run publish-storybook
```

## Testing

```sh
npm test
```

[preact]:https://preactjs.com/
[recompose]:https://github.com/acdlite/recompose
[styled-components]:https://www.styled-components.com/
[styled-system]:http://jxnblk.com/styled-system/
[husky]:https://github.com/typicode/husky