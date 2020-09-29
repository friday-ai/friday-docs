**friday-server**

> [README](../README.md) / [Globals](../globals.md) / variable

# Module: variable

## Index

### Classes

* [Variable](../classes/variable.variable-1.md)

### Interfaces

* [VariableType](../interfaces/variable.variabletype.md)

### Functions

* [create](variable.md#create)
* [destroy](variable.md#destroy)
* [getValue](variable.md#getvalue)
* [update](variable.md#update)

## Functions

### create

▸ **create**(`variable`: [VariableType](../interfaces/variable.variabletype.md)): Promise\<[VariableType](../interfaces/variable.variabletype.md)>

*Defined in [src/core/variable/variable.create.ts:20](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/variable/variable.create.ts#L20)*

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

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`variable` | [VariableType](../interfaces/variable.variabletype.md) | A variable object. |

**Returns:** Promise\<[VariableType](../interfaces/variable.variabletype.md)>

Resolve with created variable.

___

### destroy

▸ **destroy**(`id`: string): Promise\<void>

*Defined in [src/core/variable/variable.destroy.ts:13](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/variable/variable.destroy.ts#L13)*

Destroy a variable.

**`example`** 
````
friday.variable.destroy('1d99601a-cbe8-4eb0-a059-f70f53299050');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of variable. |

**Returns:** Promise\<void>

___

### getValue

▸ **getValue**(`key`: string): Promise\<[VariableType](../interfaces/variable.variabletype.md)>

*Defined in [src/core/variable/variable.getValue.ts:14](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/variable/variable.getValue.ts#L14)*

Get a variable value by key.

**`example`** 
````
friday.variable.getValue('key');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`key` | string | Key of variable. |

**Returns:** Promise\<[VariableType](../interfaces/variable.variabletype.md)>

Resolve with variable.

___

### update

▸ **update**(`idOrKey`: string, `variable`: [VariableType](../interfaces/variable.variabletype.md)): Promise\<[VariableType](../interfaces/variable.variabletype.md)>

*Defined in [src/core/variable/variable.update.ts:20](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/variable/variable.update.ts#L20)*

Update a variable.

**`example`** 
````
friday.variable.update(
'47728070-a1d2-4aaf-9930-47dc82fc1771',
{
  id: '47728070-a1d2-4aaf-9930-47dc82fc1771'
  key: 'variable update'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`idOrKey` | string | Id or key of variable |
`variable` | [VariableType](../interfaces/variable.variabletype.md) | A variable object. |

**Returns:** Promise\<[VariableType](../interfaces/variable.variabletype.md)>

Resolve with updated variable.
