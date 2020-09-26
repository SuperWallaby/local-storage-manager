# local-storage-manager

Local Sotrage Manager

A useful library when dealing with local storage. Helps to safely and neatly load object or number types.

- Typescript support
- Avoid local key value mistakes

## Usage

```ts
import LocalManager form "local-storage-manager";

type TlocalStorageKeys = "searchHookOpIndex" | "sortHookOpIndex" | "stateHookOpIndex"

const myLocalManager = LocalManager<TlocalStorageKeys>()

const {getLocal, getLocalNum, getLocalObj, saveLocal} = new LocalManager<TlocalStorageKeys>()

export {getLocal,getLocalNum,getLocalObj,saveLocal}
```

- saveLocal: save value auto stringFy
- getLocalNum : try to return numberType
- getLocal: try to return string.
- getLocalObj: try to return string Object

| name    | type                                | desc                           |
| ------- | ----------------------------------- | ------------------------------ |
| storage | : 'localStorage', 'sessionStorage'; | what kind storage will be used |
