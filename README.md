# react-hook-device-orientation :dizzy:

A React hook for detecting [device orientation](https://developer.mozilla.org/en-US/docs/Web/API/Detecting_device_orientation).

## Installation

Using `npm`:

```sh
npm install --save react-hook-device-orientation
```

Using `yarn`:

```sh
yarn add react-hook-device-orientation
```

## Usage

```jsx
import React from 'react'
import useMediaQuery from 'react-hook-device-orientation'

const ComponentWithDeviceOrientation = () => {
  const deviceOrientation = useDeviceOrientation()

  return (
    <ul>
      <li>Alpha:    {orientation.alpha}</li>
      <li>Beta:     {orientation.beta}</li>
      <li>Gamma:    {orientation.gamma}</li>
      <li>Absolute: {orientation.absolute ? 'yes' : 'no'}</li>
    </ul>
  )
}
```

## Caveats

There are slightly different implementations of the web API responsible for accessing device orientation, and therefore the values you get from this hook might not be consistent across different browsers. [Read more](https://caniuse.com/#feat=deviceorientation) about this.

## Contributions

Contributions are welcome. File bug reports, create pull requests, feel free to reach out at tothab@gmail.com.

## Licence

LGPL-3.0
