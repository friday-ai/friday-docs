> **[friday-server](../README.md)**

[Globals](../globals.md) / [variable](variable.md) /

# External module: variable

### Index

#### Classes

* [Variable](../classes/variable.variable-1.md)

#### Interfaces

* [VariableType](../interfaces/variable.variabletype.md)

#### Functions

* [create](variable.md#create)
* [destroy](variable.md#destroy)
* [getValue](variable.md#getvalue)
* [update](variable.md#update)

## Functions

###  create

▸ **create**(`variable`: [VariableType](../interfaces/variable.variabletype.md)): *`Promise<VariableType>`*

Defined in variable/variable.create.ts:21

Create a variable.

**`example`** 
````
friday.variable.create({
   id: '532aea33-3bff-479e-af74-ef678f012a51',
   key: 'key sample',
   value: 'value sample',
   owner: 'a2020069-9e06-48d9-9fa1-0b5628e612c4',
   ownerType: VariableOwner.USER
});
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`variable` | [VariableType](../interfaces/variable.variabletype.md) | A variable object. |

**Returns:** *`Promise<VariableType>`*

Resolve with created variable.

___

###  destroy

▸ **destroy**(`variable`: [VariableType](../interfaces/variable.variabletype.md)): *`Promise<void>`*

Defined in variable/variable.destroy.ts:15

Destroy a variable.

**`example`** 
````
friday.variable.destroy('1d99601a-cbe8-4eb0-a059-f70f53299050');
````

**Parameters:**

Name | Type |
------ | ------ |
`variable` | [VariableType](../interfaces/variable.variabletype.md) |

**Returns:** *`Promise<void>`*

___

###  getValue

▸ **getValue**(`key`: string): *`Promise<VariableType>`*

Defined in variable/variable.getValue.ts:15

Get a variable value by key.

**`example`** 
````
friday.variable.getValue('key');
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Key of variable. |

**Returns:** *`Promise<VariableType>`*

Resolve with variable.

___

###  update

▸ **update**(`variable`: [VariableType](../interfaces/variable.variabletype.md)): *`Promise<VariableType>`*

Defined in variable/variable.update.ts:18

Update a variable.

**`example`** 
````
friday.variable.update({
  id: '47728070-a1d2-4aaf-9930-47dc82fc1771'
  key: 'variable update'
});
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`variable` | [VariableType](../interfaces/variable.variabletype.md) | A variable object. |

**Returns:** *`Promise<VariableType>`*

Resolve with updated variable.