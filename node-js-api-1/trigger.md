**friday-server**

> [README](../README.md) / [Globals](../globals.md) / trigger

# Module: trigger

## Index

### Classes

* [Trigger](../classes/trigger.trigger-1.md)

### Interfaces

* [TriggerType](../interfaces/trigger.triggertype.md)

### Functions

* [create](trigger.md#create)
* [destroy](trigger.md#destroy)
* [getAll](trigger.md#getall)
* [getById](trigger.md#getbyid)
* [update](trigger.md#update)

## Functions

### create

▸ **create**(`trigger`: [TriggerType](../interfaces/trigger.triggertype.md)): Promise\<[TriggerType](../interfaces/trigger.triggertype.md)>

*Defined in [src/core/trigger/trigger.create.ts:23](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/trigger/trigger.create.ts#L23)*

Create a trigger.

**`example`** 
````
friday.trigger.create({
   id: '41a0c318-efe0-46c9-885b-545481a32f3d',
   name: 'Sample trigger',
   description: 'A trigger for a sample :)',
   type: AvailableConditions.DEVICE_VALUE,
   rules: JSON.stringify({
     device: '017538fb-b452-4d53-95e7-8db0bbf0d453',
     value: '23'
   })
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`trigger` | [TriggerType](../interfaces/trigger.triggertype.md) | A trigger object. |

**Returns:** Promise\<[TriggerType](../interfaces/trigger.triggertype.md)>

Resolve with created trigger.

___

### destroy

▸ **destroy**(`id`: string): Promise\<void>

*Defined in [src/core/trigger/trigger.destroy.ts:13](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/trigger/trigger.destroy.ts#L13)*

Destroy a trigger.

**`example`** 
````
friday.trigger.destroy('db35b9d3-3e6c-4b49-8988-b352494435bc');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of trigger. |

**Returns:** Promise\<void>

___

### getAll

▸ **getAll**(`options?`: GetOptions): Promise\<[TriggerType](../interfaces/trigger.triggertype.md)[]>

*Defined in [src/core/trigger/trigger.getAll.ts:25](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/trigger/trigger.getAll.ts#L25)*

Get all triggers.

**`example`** 
````
friday.trigger.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options?` | GetOptions | Options of the query. |

**Returns:** Promise\<[TriggerType](../interfaces/trigger.triggertype.md)[]>

Resolve with trigger array.

___

### getById

▸ **getById**(`id`: string, `scope?`: undefined \| string): Promise\<[TriggerType](../interfaces/trigger.triggertype.md)>

*Defined in [src/core/trigger/trigger.getById.ts:15](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/trigger/trigger.getById.ts#L15)*

Get a trigger by id.

**`example`** 
````
friday.trigger.getById('7f4bc504-16bd-4a78-aab1-48243237ab5c', 'full');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of trigger. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** Promise\<[TriggerType](../interfaces/trigger.triggertype.md)>

Resolve with trigger.

___

### update

▸ **update**(`id`: string, `trigger`: [TriggerType](../interfaces/trigger.triggertype.md)): Promise\<[TriggerType](../interfaces/trigger.triggertype.md)>

*Defined in [src/core/trigger/trigger.update.ts:20](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/trigger/trigger.update.ts#L20)*

Update a trigger.

**`example`** 
````
friday.trigger.update(
'fc5700be-8ed2-4540-a59e-a8572d8c41c5',
{
  id: 'fc5700be-8ed2-4540-a59e-a8572d8c41c5'
  name: 'trigger update'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of trigger |
`trigger` | [TriggerType](../interfaces/trigger.triggertype.md) | A trigger object. |

**Returns:** Promise\<[TriggerType](../interfaces/trigger.triggertype.md)>

Resolve with updated trigger.
