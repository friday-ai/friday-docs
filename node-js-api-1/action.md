**friday-server**

> [README](../README.md) / [Globals](../globals.md) / action

# Module: action

## Index

### Classes

* [Action](../classes/action.action-1.md)

### Interfaces

* [ActionType](../interfaces/action.actiontype.md)

### Functions

* [create](action.md#create)
* [destroy](action.md#destroy)
* [getAll](action.md#getall)
* [getById](action.md#getbyid)
* [update](action.md#update)

## Functions

### create

▸ **create**(`action`: [ActionType](../interfaces/action.actiontype.md)): Promise\<[ActionType](../interfaces/action.actiontype.md)>

*Defined in [src/core/action/action.create.ts:23](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/action/action.create.ts#L23)*

Create an action

**`example`** 
````
friday.action.create({
   id: '53dd38a4-f462-4021-a82f-92aca2aa8dea',
   name: 'action sample',
   description: 'action sample description',
   type: ActionsType.LIGHT_TURN_ON,
   subType: '',
   variableKey: 'action sample variable key',
   variableValue: 'action sample variable value',
   sceneId: '8a7823aa-8ec9-4169-b5b9-40ad52804f67'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`action` | [ActionType](../interfaces/action.actiontype.md) | An action object. |

**Returns:** Promise\<[ActionType](../interfaces/action.actiontype.md)>

Resolve with created action.

___

### destroy

▸ **destroy**(`id`: string): Promise\<void>

*Defined in [src/core/action/action.destroy.ts:13](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/action/action.destroy.ts#L13)*

Destroy an action

**`example`** 
````
friday.action.destroy('f2d7df99-8b3b-4994-86eb-400a1a951ba0');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of action. |

**Returns:** Promise\<void>

___

### getAll

▸ **getAll**(`options?`: GetOptions): Promise\<[ActionType](../interfaces/action.actiontype.md)[]>

*Defined in [src/core/action/action.getAll.ts:25](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/action/action.getAll.ts#L25)*

Get all actions

**`example`** 
````
friday.action.getAll({
    scope: '',
    take: 20,
    skip: 0
  });
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options?` | GetOptions | Options of the query. |

**Returns:** Promise\<[ActionType](../interfaces/action.actiontype.md)[]>

Resolve with action array.

___

### getById

▸ **getById**(`id`: string, `scope?`: undefined \| string): Promise\<[ActionType](../interfaces/action.actiontype.md)>

*Defined in [src/core/action/action.getById.ts:15](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/action/action.getById.ts#L15)*

Get action by id

**`example`** 
````
friday.device.getById('0480d9b4-0968-491a-8693-b1788ae0dc7d', 'full');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of action. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** Promise\<[ActionType](../interfaces/action.actiontype.md)>

Resolve with action.

___

### update

▸ **update**(`id`: string, `action`: [ActionType](../interfaces/action.actiontype.md)): Promise\<[ActionType](../interfaces/action.actiontype.md)>

*Defined in [src/core/action/action.update.ts:20](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/action/action.update.ts#L20)*

Update an action

**`example`** 
````
friday.action.update(
'16c40480-c19f-4ab5-9caf-a93a4fa1e890',
{
  id: '16c40480-c19f-4ab5-9caf-a93a4fa1e890'
  name: 'action update'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of action. |
`action` | [ActionType](../interfaces/action.actiontype.md) | An action object. |

**Returns:** Promise\<[ActionType](../interfaces/action.actiontype.md)>

Resolve with updated action.
