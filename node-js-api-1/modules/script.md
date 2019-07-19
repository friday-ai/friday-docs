> **[friday-server](../README.md)**

[Globals](../globals.md) / [script](script.md) /

# External module: script

### Index

#### Classes

* [Script](../classes/script.script-1.md)

#### Interfaces

* [ScriptType](../interfaces/script.scripttype.md)

#### Functions

* [create](script.md#create)
* [destroy](script.md#destroy)
* [getAll](script.md#getall)
* [getById](script.md#getbyid)
* [update](script.md#update)

## Functions

###  create

▸ **create**(`script`: [ScriptType](../interfaces/script.scripttype.md)): *`Promise<ScriptType>`*

Defined in script/script.create.ts:19

Create a script.

**`example`** 
````
friday.script.create({
   id: '65e0a906-8b35-49ed-87ba-e30c450a715d',
   name: 'Sample script',
   code: 'console.log(\'Hey ! This script is a sample ! :)\')'
});
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`script` | [ScriptType](../interfaces/script.scripttype.md) | A script object. |

**Returns:** *`Promise<ScriptType>`*

Resolve with created script.

___

###  destroy

▸ **destroy**(`id`: string): *`Promise<void>`*

Defined in script/script.destroy.ts:14

Destroy a script.

**`example`** 
````
friday.script.destroy('95ea9fef-5082-4851-8f3f-3fa93be2b049');
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of script. |

**Returns:** *`Promise<void>`*

___

###  getAll

▸ **getAll**(`options?`: `GetOptions`): *`Promise<ScriptType[]>`*

Defined in script/script.getAll.ts:26

Get all scripts.

**`example`** 
````
friday.script.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`options?` | `GetOptions` | Options of the query. |

**Returns:** *`Promise<ScriptType[]>`*

Resolve with script array.

___

###  getById

▸ **getById**(`id`: string, `scope?`: undefined | string): *`Promise<ScriptType>`*

Defined in script/script.getById.ts:16

Get a script by id.

**`example`** 
````
friday.script.getById('e16be2ff-9ee3-4373-8b40-9f0a2ff04ed3', 'full');
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of script. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** *`Promise<ScriptType>`*

Resolve with script.

___

###  update

▸ **update**(`script`: [ScriptType](../interfaces/script.scripttype.md)): *`Promise<ScriptType>`*

Defined in script/script.update.ts:18

Update a script.

**`example`** 
````
friday.script.update({
  id: 'fc5700be-8ed2-4540-a59e-a8572d8c41c5'
  name: 'script update'
});
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`script` | [ScriptType](../interfaces/script.scripttype.md) | A script object. |

**Returns:** *`Promise<ScriptType>`*

Resolve with updated script.