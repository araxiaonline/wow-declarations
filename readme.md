# In development Typescript declarations for AddOn / AIO devleopment for WoW Wrath of the Lich King 3.3.5a client

## Summary

**This is in development** and is specifically focused on providing accurate TypeScript definitions based on the WoW API at the time of Wrath of Lich King. 

This maintained by the Araxia team and dependendy systems: 

 - [ETS Modules](https://github.com/araxiaonline/wow-eluna-ts-module) _a content module creator specifically targets for servers running Eluna API, like Azeroth Core or Trinity Core_


**Supported transpilers for LUA targets**:

- TypescriptToLua ([GitHub-Page](https://github.com/TypeScriptToLua/TypeScriptToLua)) 

## Setup

Installing this dependency via

- `$ npm install @araxiaonline/wow-wotlk-declarations@latest` (npm repository installation)
- `$ npm install araxiaonline/wow-wotlk-declarations#` (github repository installation)

IF you are using the ETS Module System then this is bundle for you into the init command, if you you can use the following instructions below to configure your project. 

Add the wow-wotlk-declarations path to your `tsconfig.json` compiler options like below:

```js
{
    "compilerOptions": {
        // ...
        "typeRoots": [
            "./node_modules/@types",
            "./node_modules/@araxiaonline/wow-wotlk-declarations"
        ]
    }
}
```

## Changes
### Version **Dec 21 2023 - v3.3.4-3**
- Added Sound WoW Api methods
- Converted more methods from @noself to LuaMulti return types. 

### Versions **Oct 16 2023 - v3.3.5-a.1**

- Added LuaMulti to all tupleReturn methods in Cursor and UI
- Added OnDragStart and OnDragStop events to UI
- Added RegisterHypelinkClick option to FrameUI
