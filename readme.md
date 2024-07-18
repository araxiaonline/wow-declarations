[![npm version](https://badge.fury.io/js/@araxiaonline%2Fwow-wotlk-declarations.svg)](https://badge.fury.io/js/@araxiaonline%2Fwow-wotlk-declarations)
# World of Warcraft WOTLK for AddOn & AIO Development

## Summary
**This is in beta** and is specifically focused on providing accurate TypeScript definitions based on the WoW API at the time of Wrath of Lich King. 

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
### Version **Jul 17 2024** v 3.3.5-9
- Added GetRegions to Frames
- Added RegionType

### Version **Feb 5 2024** v 3.3.5-5 
- Added GetID and GetName to Tooltip
- Added MultiLua to Cursor object 

### Version **Feb 3 2024 0 v3.3.5-4**
- Added more UI Global Functions that were missing for frames
- Add Character Model Frames
- Added Model 
- Fixed some Unit returns to be LuaMulti

### Version **Dec 21 2023 - v3.3.5-3**
- Added Sound WoW Api methods
- Converted more methods from @noself to LuaMulti return types. 

### Versions **Oct 16 2023 - v3.3.5-a.1**

- Added LuaMulti to all tupleReturn methods in Cursor and UI
- Added OnDragStart and OnDragStop events to UI
- Added RegisterHypelinkClick option to FrameUI
