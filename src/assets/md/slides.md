# Virtual Dom Prototype

## Motivation

- Precursor to creating a virtual 3d scene graph
- state -> ui => state -> 3d scene graph
- An excercise to explore the inner workings of a virtual dom
- Potentially could expand into other projects

## Background

- Initial version started by following: https://medium.com/@deathmood/how-to-write-your-own-virtual-dom-ee74acc13060
- APIs should be consistent with: https://github.com/snabbdom/snabbdom

## Status

- Basic diff impl. with node/child **add**, **remove**, **replace**
- Fixed issue in article when removing multiple children
- **Hyperscript** helpers, consistent with snabbdom ...
- Basic example app arch with **rxjs**
- Class diff module initial impl.

### Structure

```sh
src/
	js/
		index.js				example app here
		ui/
			index.js			hyperscript template file
		util/
			common.js			common functions (biterate, take)
			dom.js				dom operations (select, create, remove...)
			vdom.js				our current virtual dom impl.
```


## Next steps

- Detach library from example (lib, example folders)
- Impl. attaching, diffing & patching for attrs, props & events
- Sync module and api arch with snabbdom
- Reference other vdom libraries
- Tests and benchmarks
