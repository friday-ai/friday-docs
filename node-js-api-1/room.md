**friday-server**

> [README](../README.md) / [Globals](../globals.md) / room

# Module: room

## Index

### Classes

* [Room](../classes/room.room-1.md)

### Interfaces

* [RoomType](../interfaces/room.roomtype.md)

### Functions

* [create](room.md#create)
* [destroy](room.md#destroy)
* [getAll](room.md#getall)
* [getById](room.md#getbyid)
* [update](room.md#update)

## Functions

### create

▸ **create**(`room`: [RoomType](../interfaces/room.roomtype.md)): Promise\<[RoomType](../interfaces/room.roomtype.md)>

*Defined in [src/core/room/room.create.ts:20](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/room/room.create.ts#L20)*

Create a room.

**`example`** 
````
friday.room.create({
   id: 'c1124b18-6246-4e4b-8f8b-37ec0f2af4bf',
   name: 'A room sample',
   houseId: '0f1ff0ef-3969-4de4-84bc-84fd7ab18194'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`room` | [RoomType](../interfaces/room.roomtype.md) | A room object. |

**Returns:** Promise\<[RoomType](../interfaces/room.roomtype.md)>

Resolve with created room.

___

### destroy

▸ **destroy**(`id`: string): Promise\<void>

*Defined in [src/core/room/room.destroy.ts:13](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/room/room.destroy.ts#L13)*

Destroy a room.

**`example`** 
````
friday.room.destroy('c61a79e0-fb49-43be-bd45-507864de978f');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of room. |

**Returns:** Promise\<void>

___

### getAll

▸ **getAll**(`options?`: GetOptions): Promise\<[RoomType](../interfaces/room.roomtype.md)[]>

*Defined in [src/core/room/room.getAll.ts:25](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/room/room.getAll.ts#L25)*

Get all rooms.

**`example`** 
````
friday.room.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options?` | GetOptions | Options of the query. |

**Returns:** Promise\<[RoomType](../interfaces/room.roomtype.md)[]>

Resolve with room array.

___

### getById

▸ **getById**(`id`: string, `scope?`: undefined \| string): Promise\<[RoomType](../interfaces/room.roomtype.md)>

*Defined in [src/core/room/room.getById.ts:15](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/room/room.getById.ts#L15)*

Get a room by id.

**`example`** 
````
friday.room.getById('4fdc2756-7303-47ca-b91d-6d0805165004', 'full');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of room. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** Promise\<[RoomType](../interfaces/room.roomtype.md)>

Resolve with room.

___

### update

▸ **update**(`id`: string, `room`: [RoomType](../interfaces/room.roomtype.md)): Promise\<[RoomType](../interfaces/room.roomtype.md)>

*Defined in [src/core/room/room.update.ts:20](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/room/room.update.ts#L20)*

Update a room.

**`example`** 
````
friday.room.update(
'31f61b90-27cc-4bf6-9855-4cc59526157b',
{
  id: '31f61b90-27cc-4bf6-9855-4cc59526157b'
  name: 'room update'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of room |
`room` | [RoomType](../interfaces/room.roomtype.md) | A room object. |

**Returns:** Promise\<[RoomType](../interfaces/room.roomtype.md)>

Resolve with updated room.
