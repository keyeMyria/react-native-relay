# react-native-relay

A working version of react-native with relay.

Fix the compatibility issue as described in https://github.com/facebook/relay/issues/26. 

## Getting Started

### Run graphql server

```
$ git clone https://github.com/relayjs/relay-starter-kit
$ cd relay-starter-kit
$ npm install
$ npm start
```

### Run native app

```
$ git clone https://github.com/lenaten/react-native-relay.git
$ cd react-native-relay
  set emulator/device visible graphql address in config.js
$ react-native run-android (or start ios version via xcode)
```

## Modified Packages

- react-native
  - version: 0.13.0
  - changes: 
    - https://github.com/facebook/react-native/pull/3625
    - https://github.com/lenaten/react-native-relay/commit/bd06b2a5ead23cfb66a07baccb259ccfc9e04f0c
    - rm React.Children.only constrains in react-relay/node_modules/react-static-container/lib/StaticContainer.react.js
- relay
  - version: 0.4.0
  - changes: 
    - https://github.com/skevy/relay/tree/react-native
- fbjs
  - version: 0.4.0
  - changes: 
    - https://github.com/skevy/fbjs/tree/react-native

## Thanks
- @skevy. You did the real work.
- @boourns
