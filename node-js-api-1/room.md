# room

> [**friday-server**](./)

[Globals](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/globals.md) / [room](room.md) /

## External module: room

#### Index

**Classes**

* [Room](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/classes/room.room-1.md)

**Interfaces**

* [RoomType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/room.roomtype.md)

**Functions**

* [create](room.md#create)
* [destroy](room.md#destroy)
* [getAll](room.md#getall)
* [getById](room.md#getbyid)
* [update](room.md#update)

### Functions

#### create

▸ **create**\(`room`: [RoomType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/room.roomtype.md)\): _`Promise<RoomType>`_

Defined in room/room.create.ts:19

Create a room.

**`example`**

```text
friday.room.create({
   id: 'c1124b18-6246-4e4b-8f8b-37ec0f2af4bf',
   name: 'A room sample',
   houseId: '0f1ff0ef-3969-4de4-84bc-84fd7ab18194'
});
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `room` | [RoomType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/room.roomtype.md) | A room object. |

**Returns:** _`Promise<RoomType>`_

Resolve with created room.

#### destroy

▸ **destroy**\(`id`: string\): _`Promise<void>`_

Defined in room/room.destroy.ts:14

Destroy a room.

**`example`**

```text
friday.room.destroy('c61a79e0-fb49-43be-bd45-507864de978f');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `id` | string | Id of room. |

**Returns:** _`Promise<void>`_

#### getAll

▸ **getAll**\(`options?`: `GetOptions`\): _`Promise<RoomType[]>`_

Defined in room/room.getAll.ts:26

Get all rooms.

**`example`**

```text
friday.room.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `options?` | `GetOptions` | Options of the query. |

**Returns:** _`Promise<RoomType[]>`_

Resolve with room array.

#### getById

▸ **getById**\(`id`: string, `scope?`: undefined \| string\): _`Promise<RoomType>`_

Defined in room/room.getById.ts:16

Get a room by id.

**`example`**

```text
friday.room.getById('4fdc2756-7303-47ca-b91d-6d0805165004', 'full');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `id` | string | Id of room. |
| `scope?` | undefined \| string | Scope option. \(Optional\) |

**Returns:** _`Promise<RoomType>`_

Resolve with room.

#### update

▸ **update**\(`room`: [RoomType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/room.roomtype.md)\): _`Promise<RoomType>`_

Defined in room/room.update.ts:18

Update a room.

**`example`**

```text
friday.room.update({
  id: '31f61b90-27cc-4bf6-9855-4cc59526157b'
  name: 'room update'
});
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `room` | [RoomType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/room.roomtype.md) | A room object. |

**Returns:** _`Promise<RoomType>`_

Resolve with updated room.

