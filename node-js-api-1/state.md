**friday-server**

> [README](../README.md) / [Globals](../globals.md) / state

# Module: state

## Index

### Classes

* [State](../classes/state.state-1.md)

### Interfaces

* [StateType](../interfaces/state.statetype.md)

### Functions

* [getByOwner](state.md#getbyowner)
* [purge](state.md#purge)
* [set](state.md#set)

## Functions

### getByOwner

▸ **getByOwner**(`owner`: string): Promise\<[StateType](../interfaces/state.statetype.md)>

*Defined in [src/core/state/state.getByOwner.ts:14](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/state/state.getByOwner.ts#L14)*

Get a state by owner.

**`example`** 
````
friday.state.getByOwner('88e5b907-d62d-433c-8811-999c9ed72453')
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`owner` | string | Id of owner. |

**Returns:** Promise\<[StateType](../interfaces/state.statetype.md)>

Resolve with state.

___

### purge

▸ **purge**(`this`: StateClass): Promise\<void>

*Defined in [src/core/state/state.purge.ts:14](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/state/state.purge.ts#L14)*

Purge states.

**`example`** 
````
friday.state.purge();
````

#### Parameters:

Name | Type |
------ | ------ |
`this` | StateClass |

**Returns:** Promise\<void>

___

### set

▸ **set**(`state`: [StateType](../interfaces/state.statetype.md)): Promise\<[StateType](../interfaces/state.statetype.md)>

*Defined in [src/core/state/state.set.ts:19](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/state/state.set.ts#L19)*

Set a state.

**`example`** 
````
friday.state.set({
  id: '9a05e6c3-e36a-4779-bc66-6f7d015920c7',
  owner: '0cd30aef-9c4e-4a23-81e3-3547971296e5',
  ownerType: StateOwner.USER,
  value: AvailableState.USER_AT_HOME
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`state` | [StateType](../interfaces/state.statetype.md) | -A state object. |

**Returns:** Promise\<[StateType](../interfaces/state.statetype.md)>

Resolve with state.
