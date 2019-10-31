# scene

> [**friday-server**](./)

[Globals](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/globals.md) / [scene](scene.md) /

## External module: scene

#### Index

**Classes**

* [Scene](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/classes/scene.scene-1.md)

**Interfaces**

* [SceneType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/scene.scenetype.md)

**Functions**

* [create](scene.md#create)
* [destroy](scene.md#destroy)
* [getAll](scene.md#getall)
* [getById](scene.md#getbyid)
* [update](scene.md#update)

### Functions

#### create

▸ **create**\(`scene`: [SceneType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/scene.scenetype.md)\): _`Promise<SceneType>`_

Defined in scene/scene.create.ts:19

Create a scene.

**`example`**

```text
friday.scene.create({
   id: 'e49c0809-7f51-4f0c-842f-36461b7bd18a',
   name: 'Sample scene',
   description: 'A sample to create a scene'
});
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `scene` | [SceneType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/scene.scenetype.md) | A scene object. |

**Returns:** _`Promise<SceneType>`_

Resolve with created scene.

#### destroy

▸ **destroy**\(`id`: string\): _`Promise<void>`_

Defined in scene/scene.destroy.ts:14

Destroy a scene.

**`example`**

```text
friday.scene.destroy('36707443-fba9-4fbd-9aa6-4715f5a63ff9');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `id` | string | Id of scene. |

**Returns:** _`Promise<void>`_

#### getAll

▸ **getAll**\(`options?`: `GetOptions`\): _`Promise<SceneType[]>`_

Defined in scene/scene.getAll.ts:26

Get all scenes.

**`example`**

```text
friday.scene.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `options?` | `GetOptions` | Options of the query. |

**Returns:** _`Promise<SceneType[]>`_

Resolve with scene array.

#### getById

▸ **getById**\(`id`: string, `scope?`: undefined \| string\): _`Promise<SceneType>`_

Defined in scene/scene.getById.ts:16

Get a scene by id.

**`example`**

```text
friday.scene.getById('d0766a83-68e7-44aa-9124-f8e5fa137304', 'full');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `id` | string | Id of scene. |
| `scope?` | undefined \| string | Scope option. \(Optional\) |

**Returns:** _`Promise<SceneType>`_

Resolve with scene.

#### update

▸ **update**\(`scene`: [SceneType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/scene.scenetype.md)\): _`Promise<SceneType>`_

Defined in scene/scene.update.ts:18

Update a scene.

**`example`**

```text
friday.scene.update({
  id: '30967a17-8e13-4460-afa0-1069fa890c4e'
  name: 'scene update'
});
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `scene` | [SceneType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/scene.scenetype.md) | A scene object. |

**Returns:** _`Promise<SceneType>`_

Resolve with updated scene.

