> **[friday-server](../README.md)**

[Globals](../globals.md) / [state](state.md) /

# External module: state

### Index

#### Classes

* [State](../classes/state.state-1.md)

#### Interfaces

* [StateType](../interfaces/state.statetype.md)

#### Functions

* [create](state.md#create)
* [getByOwner](state.md#getbyowner)

## Functions

###  create

▸ **create**(`state`: [StateType](../interfaces/state.statetype.md)): *`Promise<StateType>`*

Defined in state/state.set.ts:20

Set a state.

**`example`** 
````
friday.state.getByOwner({
  id: '9a05e6c3-e36a-4779-bc66-6f7d015920c7',
  owner: '0cd30aef-9c4e-4a23-81e3-3547971296e5',
  ownerType: StateOwner.USER,
  value: AvailableState.USER_AT_HOME
};
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`state` | [StateType](../interfaces/state.statetype.md) | -A state object. |

**Returns:** *`Promise<StateType>`*

Resolve with state.

___

###  getByOwner

▸ **getByOwner**(`owner`: string): *`Promise<StateType>`*

Defined in state/state.getByOwner.ts:15

Get a state by owner.

**`example`** 
````
friday.state.getByOwner('88e5b907-d62d-433c-8811-999c9ed72453')
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`owner` | string | Id of owner. |

**Returns:** *`Promise<StateType>`*

Resolve with state.