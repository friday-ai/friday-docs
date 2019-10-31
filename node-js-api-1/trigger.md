# trigger

> [**friday-server**](./)

[Globals](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/globals.md) / [trigger](trigger.md) /

## External module: trigger

#### Index

**Classes**

* [Trigger](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/classes/trigger.trigger-1.md)

**Interfaces**

* [TriggerType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/trigger.triggertype.md)

**Functions**

* [create](trigger.md#create)
* [destroy](trigger.md#destroy)
* [getAll](trigger.md#getall)
* [getById](trigger.md#getbyid)
* [update](trigger.md#update)

### Functions

#### create

▸ **create**\(`trigger`: [TriggerType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/trigger.triggertype.md)\): _`Promise<TriggerType>`_

Defined in trigger/trigger.create.ts:24

Create a trigger.

**`example`**

```text
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
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `trigger` | [TriggerType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/trigger.triggertype.md) | A trigger object. |

**Returns:** _`Promise<TriggerType>`_

Resolve with created trigger.

#### destroy

▸ **destroy**\(`id`: string\): _`Promise<void>`_

Defined in trigger/trigger.destroy.ts:14

Destroy a trigger.

**`example`**

```text
friday.trigger.destroy('db35b9d3-3e6c-4b49-8988-b352494435bc');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `id` | string | Id of trigger. |

**Returns:** _`Promise<void>`_

#### getAll

▸ **getAll**\(`options?`: `GetOptions`\): _`Promise<TriggerType[]>`_

Defined in trigger/trigger.getAll.ts:26

Get all triggers.

**`example`**

```text
friday.trigger.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `options?` | `GetOptions` | Options of the query. |

**Returns:** _`Promise<TriggerType[]>`_

Resolve with trigger array.

#### getById

▸ **getById**\(`id`: string, `scope?`: undefined \| string\): _`Promise<TriggerType>`_

Defined in trigger/trigger.getById.ts:16

Get a trigger by id.

**`example`**

```text
friday.trigger.getById('7f4bc504-16bd-4a78-aab1-48243237ab5c', 'full');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `id` | string | Id of trigger. |
| `scope?` | undefined \| string | Scope option. \(Optional\) |

**Returns:** _`Promise<TriggerType>`_

Resolve with trigger.

#### update

▸ **update**\(`trigger`: [TriggerType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/trigger.triggertype.md)\): _`Promise<TriggerType>`_

Defined in trigger/trigger.update.ts:18

Update a trigger.

**`example`**

```text
friday.trigger.update({
  id: 'fc5700be-8ed2-4540-a59e-a8572d8c41c5'
  name: 'trigger update'
});
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `trigger` | [TriggerType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/trigger.triggertype.md) | A trigger object. |

**Returns:** _`Promise<TriggerType>`_

Resolve with updated trigger.

