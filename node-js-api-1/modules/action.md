> **[friday-server](../README.md)**

[Globals](../globals.md) / [action](action.md) /

# External module: action

### Index

#### Classes

* [Action](../classes/action.action-1.md)

#### Interfaces

* [ActionType](../interfaces/action.actiontype.md)

#### Functions

* [create](action.md#create)
* [destroy](action.md#destroy)
* [getAll](action.md#getall)
* [getById](action.md#getbyid)
* [update](action.md#update)

## Functions

###  create

▸ **create**(`action`: [ActionType](../interfaces/action.actiontype.md)): *`Promise<ActionType>`*

Defined in action/action.create.ts:25

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

**`memberof`** Action

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`action` | [ActionType](../interfaces/action.actiontype.md) | An action object. |

**Returns:** *`Promise<ActionType>`*

Resolve with created action.

___

###  destroy

▸ **destroy**(`id`: string): *`Promise<void>`*

Defined in action/action.destroy.ts:14

Destroy an action

**`example`** 
````
friday.action.destroy('f2d7df99-8b3b-4994-86eb-400a1a951ba0');
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of action. |

**Returns:** *`Promise<void>`*

___

###  getAll

▸ **getAll**(`options?`: `GetOptions`): *`Promise<ActionType[]>`*

Defined in action/action.getAll.ts:26

Get all actions

**`example`** 
````
friday.action.getAll({
    scope: '',
    take: 20,
    skip: 0
  });
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`options?` | `GetOptions` | Options of the query. |

**Returns:** *`Promise<ActionType[]>`*

Resolve with action array.

___

###  getById

▸ **getById**(`id`: string, `scope?`: undefined | string): *`Promise<ActionType>`*

Defined in action/action.getById.ts:16

Get action by id

**`example`** 
````
friday.device.getById('0480d9b4-0968-491a-8693-b1788ae0dc7d', 'full');
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of action. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** *`Promise<ActionType>`*

Resolve with action.

___

###  update

▸ **update**(`action`: [ActionType](../interfaces/action.actiontype.md)): *`Promise<ActionType>`*

Defined in action/action.update.ts:18

Update an action

**`example`** 
````
friday.action.update({
  id: '16c40480-c19f-4ab5-9caf-a93a4fa1e890'
  name: 'action update'
});
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`action` | [ActionType](../interfaces/action.actiontype.md) | An action object. |

**Returns:** *`Promise<ActionType>`*

Resolve with updated action.