> **[friday-server](../README.md)**

[Globals](../globals.md) / [house](house.md) /

# External module: house

### Index

#### Classes

* [House](../classes/house.house-1.md)

#### Interfaces

* [HouseType](../interfaces/house.housetype.md)

#### Functions

* [create](house.md#create)
* [destroy](house.md#destroy)
* [getAll](house.md#getall)
* [getById](house.md#getbyid)
* [update](house.md#update)

## Functions

###  create

▸ **create**(`house`: [HouseType](../interfaces/house.housetype.md)): *`Promise<HouseType>`*

Defined in house/house.create.ts:20

Create an house.

**`example`** 
````
friday.house.create({
   id: '7774f404-1947-4908-b2a4-5ab5df808693',
   name: 'Sample House',
   latitude: '34.0012295',
   longitude: '-118.8067245'
});
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`house` | [HouseType](../interfaces/house.housetype.md) | An house object. |

**Returns:** *`Promise<HouseType>`*

Resolve with created house.

___

###  destroy

▸ **destroy**(`id`: string): *`Promise<void>`*

Defined in house/house.destroy.ts:14

Destroy an house.

**`example`** 
````
friday.house.destroy('d5988c5b-c3ae-4aff-ab63-037d855c1978');
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of house. |

**Returns:** *`Promise<void>`*

___

###  getAll

▸ **getAll**(`options?`: `GetOptions`): *`Promise<HouseType[]>`*

Defined in house/house.getAll.ts:26

Get all houses.

**`example`** 
````
friday.house.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`options?` | `GetOptions` | Options of the query. |

**Returns:** *`Promise<HouseType[]>`*

Resolve with house array.

___

###  getById

▸ **getById**(`id`: string, `scope?`: undefined | string): *`Promise<HouseType>`*

Defined in house/house.getById.ts:16

Get a house by id.

**`example`** 
````
friday.device.getById('6be1d66d-da22-47c2-b7d0-54b51429db62', 'full');
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of house. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** *`Promise<HouseType>`*

Resolve with house.

___

###  update

▸ **update**(`house`: [HouseType](../interfaces/house.housetype.md)): *`Promise<HouseType>`*

Defined in house/house.update.ts:18

Update an house.

**`example`** 
````
friday.house.update({
  id: '40d43cf1-2127-41e9-ac69-9e39636fac20'
  name: 'house update'
});
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`house` | [HouseType](../interfaces/house.housetype.md) | An house object. |

**Returns:** *`Promise<HouseType>`*

Resolve with updated house.