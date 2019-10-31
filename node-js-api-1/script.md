# script

> [**friday-server**](./)

[Globals](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/globals.md) / [script](script.md) /

## External module: script

#### Index

**Classes**

* [Script](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/classes/script.script-1.md)

**Interfaces**

* [ScriptType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/script.scripttype.md)

**Functions**

* [create](script.md#create)
* [destroy](script.md#destroy)
* [getAll](script.md#getall)
* [getById](script.md#getbyid)
* [update](script.md#update)

### Functions

#### create

▸ **create**\(`script`: [ScriptType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/script.scripttype.md)\): _`Promise<ScriptType>`_

Defined in script/script.create.ts:19

Create a script.

**`example`**

```text
friday.script.create({
   id: '65e0a906-8b35-49ed-87ba-e30c450a715d',
   name: 'Sample script',
   code: 'console.log(\'Hey ! This script is a sample ! :)\')'
});
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `script` | [ScriptType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/script.scripttype.md) | A script object. |

**Returns:** _`Promise<ScriptType>`_

Resolve with created script.

#### destroy

▸ **destroy**\(`id`: string\): _`Promise<void>`_

Defined in script/script.destroy.ts:14

Destroy a script.

**`example`**

```text
friday.script.destroy('95ea9fef-5082-4851-8f3f-3fa93be2b049');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `id` | string | Id of script. |

**Returns:** _`Promise<void>`_

#### getAll

▸ **getAll**\(`options?`: `GetOptions`\): _`Promise<ScriptType[]>`_

Defined in script/script.getAll.ts:26

Get all scripts.

**`example`**

```text
friday.script.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `options?` | `GetOptions` | Options of the query. |

**Returns:** _`Promise<ScriptType[]>`_

Resolve with script array.

#### getById

▸ **getById**\(`id`: string, `scope?`: undefined \| string\): _`Promise<ScriptType>`_

Defined in script/script.getById.ts:16

Get a script by id.

**`example`**

```text
friday.script.getById('e16be2ff-9ee3-4373-8b40-9f0a2ff04ed3', 'full');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `id` | string | Id of script. |
| `scope?` | undefined \| string | Scope option. \(Optional\) |

**Returns:** _`Promise<ScriptType>`_

Resolve with script.

#### update

▸ **update**\(`script`: [ScriptType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/script.scripttype.md)\): _`Promise<ScriptType>`_

Defined in script/script.update.ts:18

Update a script.

**`example`**

```text
friday.script.update({
  id: 'fc5700be-8ed2-4540-a59e-a8572d8c41c5'
  name: 'script update'
});
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `script` | [ScriptType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/script.scripttype.md) | A script object. |

**Returns:** _`Promise<ScriptType>`_

Resolve with updated script.

