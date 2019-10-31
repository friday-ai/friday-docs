# state

> [**friday-server**](./)

[Globals](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/globals.md) / [state](state.md) /

## External module: state

#### Index

**Classes**

* [State](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/classes/state.state-1.md)

**Interfaces**

* [StateType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/state.statetype.md)

**Functions**

* [create](state.md#create)
* [getByOwner](state.md#getbyowner)

### Functions

#### create

▸ **create**\(`state`: [StateType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/state.statetype.md)\): _`Promise<StateType>`_

Defined in state/state.set.ts:20

Set a state.

**`example`**

```text
friday.state.getByOwner({
  id: '9a05e6c3-e36a-4779-bc66-6f7d015920c7',
  owner: '0cd30aef-9c4e-4a23-81e3-3547971296e5',
  ownerType: StateOwner.USER,
  value: AvailableState.USER_AT_HOME
};
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `state` | [StateType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/state.statetype.md) | -A state object. |

**Returns:** _`Promise<StateType>`_

Resolve with state.

#### getByOwner

▸ **getByOwner**\(`owner`: string\): _`Promise<StateType>`_

Defined in state/state.getByOwner.ts:15

Get a state by owner.

**`example`**

```text
friday.state.getByOwner('88e5b907-d62d-433c-8811-999c9ed72453')
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `owner` | string | Id of owner. |

**Returns:** _`Promise<StateType>`_

Resolve with state.

