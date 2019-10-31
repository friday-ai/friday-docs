# variable

> [**friday-server**](./)

[Globals](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/globals.md) / [variable](variable.md) /

## External module: variable

#### Index

**Classes**

* [Variable](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/classes/variable.variable-1.md)

**Interfaces**

* [VariableType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/variable.variabletype.md)

**Functions**

* [create](variable.md#create)
* [destroy](variable.md#destroy)
* [getValue](variable.md#getvalue)
* [update](variable.md#update)

### Functions

#### create

▸ **create**\(`variable`: [VariableType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/variable.variabletype.md)\): _`Promise<VariableType>`_

Defined in variable/variable.create.ts:21

Create a variable.

**`example`**

```text
friday.variable.create({
   id: '532aea33-3bff-479e-af74-ef678f012a51',
   key: 'key sample',
   value: 'value sample',
   owner: 'a2020069-9e06-48d9-9fa1-0b5628e612c4',
   ownerType: VariableOwner.USER
});
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `variable` | [VariableType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/variable.variabletype.md) | A variable object. |

**Returns:** _`Promise<VariableType>`_

Resolve with created variable.

#### destroy

▸ **destroy**\(`variable`: [VariableType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/variable.variabletype.md)\): _`Promise<void>`_

Defined in variable/variable.destroy.ts:15

Destroy a variable.

**`example`**

```text
friday.variable.destroy('1d99601a-cbe8-4eb0-a059-f70f53299050');
```

**Parameters:**

| Name | Type |
| :--- | :--- |
| `variable` | [VariableType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/variable.variabletype.md) |

**Returns:** _`Promise<void>`_

#### getValue

▸ **getValue**\(`key`: string\): _`Promise<VariableType>`_

Defined in variable/variable.getValue.ts:15

Get a variable value by key.

**`example`**

```text
friday.variable.getValue('key');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `key` | string | Key of variable. |

**Returns:** _`Promise<VariableType>`_

Resolve with variable.

#### update

▸ **update**\(`variable`: [VariableType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/variable.variabletype.md)\): _`Promise<VariableType>`_

Defined in variable/variable.update.ts:18

Update a variable.

**`example`**

```text
friday.variable.update({
  id: '47728070-a1d2-4aaf-9930-47dc82fc1771'
  key: 'variable update'
});
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `variable` | [VariableType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/variable.variabletype.md) | A variable object. |

**Returns:** _`Promise<VariableType>`_

Resolve with updated variable.

