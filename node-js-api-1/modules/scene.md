> **[friday-server](../README.md)**

[Globals](../globals.md) / [scene](scene.md) /

# External module: scene

### Index

#### Classes

* [Scene](../classes/scene.scene-1.md)

#### Interfaces

* [SceneType](../interfaces/scene.scenetype.md)

#### Functions

* [create](scene.md#create)
* [destroy](scene.md#destroy)
* [getAll](scene.md#getall)
* [getById](scene.md#getbyid)
* [update](scene.md#update)

## Functions

###  create

▸ **create**(`scene`: [SceneType](../interfaces/scene.scenetype.md)): *`Promise<SceneType>`*

Defined in scene/scene.create.ts:19

Create a scene.

**`example`** 
````
friday.scene.create({
   id: 'e49c0809-7f51-4f0c-842f-36461b7bd18a',
   name: 'Sample scene',
   description: 'A sample to create a scene'
});
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`scene` | [SceneType](../interfaces/scene.scenetype.md) | A scene object. |

**Returns:** *`Promise<SceneType>`*

Resolve with created scene.

___

###  destroy

▸ **destroy**(`id`: string): *`Promise<void>`*

Defined in scene/scene.destroy.ts:14

Destroy a scene.

**`example`** 
````
friday.scene.destroy('36707443-fba9-4fbd-9aa6-4715f5a63ff9');
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of scene. |

**Returns:** *`Promise<void>`*

___

###  getAll

▸ **getAll**(`options?`: `GetOptions`): *`Promise<SceneType[]>`*

Defined in scene/scene.getAll.ts:26

Get all scenes.

**`example`** 
````
friday.scene.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`options?` | `GetOptions` | Options of the query. |

**Returns:** *`Promise<SceneType[]>`*

Resolve with scene array.

___

###  getById

▸ **getById**(`id`: string, `scope?`: undefined | string): *`Promise<SceneType>`*

Defined in scene/scene.getById.ts:16

Get a scene by id.

**`example`** 
````
friday.scene.getById('d0766a83-68e7-44aa-9124-f8e5fa137304', 'full');
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of scene. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** *`Promise<SceneType>`*

Resolve with scene.

___

###  update

▸ **update**(`scene`: [SceneType](../interfaces/scene.scenetype.md)): *`Promise<SceneType>`*

Defined in scene/scene.update.ts:18

Update a scene.

**`example`** 
````
friday.scene.update({
  id: '30967a17-8e13-4460-afa0-1069fa890c4e'
  name: 'scene update'
});
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`scene` | [SceneType](../interfaces/scene.scenetype.md) | A scene object. |

**Returns:** *`Promise<SceneType>`*

Resolve with updated scene.