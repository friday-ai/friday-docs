**friday-server**

> [README](../README.md) / [Globals](../globals.md) / script

# Module: script

## Index

### Classes

* [Script](../classes/script.script-1.md)

### Interfaces

* [ScriptType](../interfaces/script.scripttype.md)

### Functions

* [create](script.md#create)
* [destroy](script.md#destroy)
* [getAll](script.md#getall)
* [getById](script.md#getbyid)
* [update](script.md#update)

## Functions

### create

▸ **create**(`script`: [ScriptType](../interfaces/script.scripttype.md)): Promise\<[ScriptType](../interfaces/script.scripttype.md)>

*Defined in [src/core/script/script.create.ts:18](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/script/script.create.ts#L18)*

Create a script.

**`example`** 
````
friday.script.create({
   id: '65e0a906-8b35-49ed-87ba-e30c450a715d',
   name: 'Sample script',
   code: 'console.log(\'Hey ! This script is a sample ! :)\')'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`script` | [ScriptType](../interfaces/script.scripttype.md) | A script object. |

**Returns:** Promise\<[ScriptType](../interfaces/script.scripttype.md)>

Resolve with created script.

___

### destroy

▸ **destroy**(`id`: string): Promise\<void>

*Defined in [src/core/script/script.destroy.ts:13](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/script/script.destroy.ts#L13)*

Destroy a script.

**`example`** 
````
friday.script.destroy('95ea9fef-5082-4851-8f3f-3fa93be2b049');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of script. |

**Returns:** Promise\<void>

___

### getAll

▸ **getAll**(`options?`: GetOptions): Promise\<[ScriptType](../interfaces/script.scripttype.md)[]>

*Defined in [src/core/script/script.getAll.ts:25](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/script/script.getAll.ts#L25)*

Get all scripts.

**`example`** 
````
friday.script.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options?` | GetOptions | Options of the query. |

**Returns:** Promise\<[ScriptType](../interfaces/script.scripttype.md)[]>

Resolve with script array.

___

### getById

▸ **getById**(`id`: string): Promise\<[ScriptType](../interfaces/script.scripttype.md)>

*Defined in [src/core/script/script.getById.ts:14](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/script/script.getById.ts#L14)*

Get a script by id.

**`example`** 
````
friday.script.getById('e16be2ff-9ee3-4373-8b40-9f0a2ff04ed3', 'full');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of script. |

**Returns:** Promise\<[ScriptType](../interfaces/script.scripttype.md)>

Resolve with script.

___

### update

▸ **update**(`id`: string, `script`: [ScriptType](../interfaces/script.scripttype.md)): Promise\<[ScriptType](../interfaces/script.scripttype.md)>

*Defined in [src/core/script/script.update.ts:20](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/script/script.update.ts#L20)*

Update a script.

**`example`** 
````
friday.script.update(
'fc5700be-8ed2-4540-a59e-a8572d8c41c5',
{
  id: 'fc5700be-8ed2-4540-a59e-a8572d8c41c5'
  name: 'script update'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of script |
`script` | [ScriptType](../interfaces/script.scripttype.md) | A script object. |

**Returns:** Promise\<[ScriptType](../interfaces/script.scripttype.md)>

Resolve with updated script.
