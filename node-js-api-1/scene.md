**friday-server**

> [README](../README.md) / [Globals](../globals.md) / scene

# Module: scene

## Index

### Classes

* [Scene](../classes/scene.scene-1.md)

### Interfaces

* [SceneType](../interfaces/scene.scenetype.md)

### Functions

* [create](scene.md#create)
* [destroy](scene.md#destroy)
* [getAll](scene.md#getall)
* [getById](scene.md#getbyid)
* [update](scene.md#update)

## Functions

### create

▸ **create**(`scene`: [SceneType](../interfaces/scene.scenetype.md)): Promise\<[SceneType](../interfaces/scene.scenetype.md)>

*Defined in [src/core/scene/scene.create.ts:18](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/scene/scene.create.ts#L18)*

Create a scene.

**`example`** 
````
friday.scene.create({
   id: 'e49c0809-7f51-4f0c-842f-36461b7bd18a',
   name: 'Sample scene',
   description: 'A sample to create a scene'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`scene` | [SceneType](../interfaces/scene.scenetype.md) | A scene object. |

**Returns:** Promise\<[SceneType](../interfaces/scene.scenetype.md)>

Resolve with created scene.

___

### destroy

▸ **destroy**(`id`: string): Promise\<void>

*Defined in [src/core/scene/scene.destroy.ts:13](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/scene/scene.destroy.ts#L13)*

Destroy a scene.

**`example`** 
````
friday.scene.destroy('36707443-fba9-4fbd-9aa6-4715f5a63ff9');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of scene. |

**Returns:** Promise\<void>

___

### getAll

▸ **getAll**(`options?`: GetOptions): Promise\<[SceneType](../interfaces/scene.scenetype.md)[]>

*Defined in [src/core/scene/scene.getAll.ts:25](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/scene/scene.getAll.ts#L25)*

Get all scenes.

**`example`** 
````
friday.scene.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options?` | GetOptions | Options of the query. |

**Returns:** Promise\<[SceneType](../interfaces/scene.scenetype.md)[]>

Resolve with scene array.

___

### getById

▸ **getById**(`id`: string, `scope?`: undefined \| string): Promise\<[SceneType](../interfaces/scene.scenetype.md)>

*Defined in [src/core/scene/scene.getById.ts:15](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/scene/scene.getById.ts#L15)*

Get a scene by id.

**`example`** 
````
friday.scene.getById('d0766a83-68e7-44aa-9124-f8e5fa137304', 'full');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of scene. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** Promise\<[SceneType](../interfaces/scene.scenetype.md)>

Resolve with scene.

___

### update

▸ **update**(`id`: string, `scene`: [SceneType](../interfaces/scene.scenetype.md)): Promise\<[SceneType](../interfaces/scene.scenetype.md)>

*Defined in [src/core/scene/scene.update.ts:20](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/scene/scene.update.ts#L20)*

Update a scene.

**`example`** 
````
friday.scene.update(
'30967a17-8e13-4460-afa0-1069fa890c4e',
{
  id: '30967a17-8e13-4460-afa0-1069fa890c4e'
  name: 'scene update'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of scene |
`scene` | [SceneType](../interfaces/scene.scenetype.md) | A scene object. |

**Returns:** Promise\<[SceneType](../interfaces/scene.scenetype.md)>

Resolve with updated scene.
