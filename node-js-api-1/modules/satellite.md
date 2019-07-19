> **[friday-server](../README.md)**

[Globals](../globals.md) / [satellite](satellite.md) /

# External module: satellite

### Index

#### Classes

* [Satellite](../classes/satellite.satellite-1.md)

#### Interfaces

* [SatelliteType](../interfaces/satellite.satellitetype.md)

#### Functions

* [create](satellite.md#create)
* [destroy](satellite.md#destroy)
* [getAll](satellite.md#getall)
* [getById](satellite.md#getbyid)
* [update](satellite.md#update)

## Functions

###  create

▸ **create**(`satellite`: [SatelliteType](../interfaces/satellite.satellitetype.md)): *`Promise<SatelliteType>`*

Defined in satellite/satellite.create.ts:19

Create a satellite.

**`example`** 
````
friday.satellite.create({
   id: '70d24472-24bb-4419-89da-dfd7dd30aa5d',
   name: 'Satellite sample',
   roomId: '202e512f-a02a-4fc3-a96d-cd639dd03556'
});
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`satellite` | [SatelliteType](../interfaces/satellite.satellitetype.md) | A satellite object. |

**Returns:** *`Promise<SatelliteType>`*

Resolve with created satellite.

___

###  destroy

▸ **destroy**(`id`: string): *`Promise<void>`*

Defined in satellite/satellite.destroy.ts:14

Destroy a satellite.

**`example`** 
````
friday.satellite.destroy('ac21d402-35a9-4cbc-8ea9-33a2cff93b7a');
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of satellite. |

**Returns:** *`Promise<void>`*

___

###  getAll

▸ **getAll**(`options?`: `GetOptions`): *`Promise<SatelliteType[]>`*

Defined in satellite/satellite.getAll.ts:26

Get all satellites.

**`example`** 
````
friday.satellite.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`options?` | `GetOptions` | Options of the query. |

**Returns:** *`Promise<SatelliteType[]>`*

Resolve with satellite array.

___

###  getById

▸ **getById**(`id`: string, `scope?`: undefined | string): *`Promise<SatelliteType>`*

Defined in satellite/satellite.getById.ts:16

Get a satellite by id.

**`example`** 
````
friday.satellite.getById('d30cad70-503a-43ed-8913-c80a80c5ba6a', 'full');
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of satellite. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** *`Promise<SatelliteType>`*

Resolve with satellite.

___

###  update

▸ **update**(`satellite`: [SatelliteType](../interfaces/satellite.satellitetype.md)): *`Promise<SatelliteType>`*

Defined in satellite/satellite.update.ts:18

Update a satellite.

**`example`** 
````
friday.satellite.update({
  id: '31f61b90-27cc-4bf6-9855-4cc59526157b'
  name: 'satellite update'
});
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`satellite` | [SatelliteType](../interfaces/satellite.satellitetype.md) | A satellite object. |

**Returns:** *`Promise<SatelliteType>`*

Resolve with updated satellite.