**friday-server**

> [README](../README.md) / [Globals](../globals.md) / satellite

# Module: satellite

## Index

### Classes

* [Satellite](../classes/satellite.satellite-1.md)

### Interfaces

* [SatelliteType](../interfaces/satellite.satellitetype.md)

### Functions

* [create](satellite.md#create)
* [destroy](satellite.md#destroy)
* [getAll](satellite.md#getall)
* [getById](satellite.md#getbyid)
* [update](satellite.md#update)

## Functions

### create

▸ **create**(`satellite`: [SatelliteType](../interfaces/satellite.satellitetype.md)): Promise\<[SatelliteType](../interfaces/satellite.satellitetype.md)>

*Defined in [src/core/satellite/satellite.create.ts:20](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/satellite/satellite.create.ts#L20)*

Create a satellite.

**`example`** 
````
friday.satellite.create({
   id: '70d24472-24bb-4419-89da-dfd7dd30aa5d',
   name: 'Satellite sample',
   roomId: '202e512f-a02a-4fc3-a96d-cd639dd03556'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`satellite` | [SatelliteType](../interfaces/satellite.satellitetype.md) | A satellite object. |

**Returns:** Promise\<[SatelliteType](../interfaces/satellite.satellitetype.md)>

Resolve with created satellite.

___

### destroy

▸ **destroy**(`id`: string): Promise\<void>

*Defined in [src/core/satellite/satellite.destroy.ts:13](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/satellite/satellite.destroy.ts#L13)*

Destroy a satellite.

**`example`** 
````
friday.satellite.destroy('ac21d402-35a9-4cbc-8ea9-33a2cff93b7a');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of satellite. |

**Returns:** Promise\<void>

___

### getAll

▸ **getAll**(`options?`: GetOptions): Promise\<[SatelliteType](../interfaces/satellite.satellitetype.md)[]>

*Defined in [src/core/satellite/satellite.getAll.ts:25](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/satellite/satellite.getAll.ts#L25)*

Get all satellites.

**`example`** 
````
friday.satellite.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`options?` | GetOptions | Options of the query. |

**Returns:** Promise\<[SatelliteType](../interfaces/satellite.satellitetype.md)[]>

Resolve with satellite array.

___

### getById

▸ **getById**(`id`: string, `scope?`: undefined \| string): Promise\<[SatelliteType](../interfaces/satellite.satellitetype.md)>

*Defined in [src/core/satellite/satellite.getById.ts:15](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/satellite/satellite.getById.ts#L15)*

Get a satellite by id.

**`example`** 
````
friday.satellite.getById('d30cad70-503a-43ed-8913-c80a80c5ba6a', 'full');
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of satellite. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** Promise\<[SatelliteType](../interfaces/satellite.satellitetype.md)>

Resolve with satellite.

___

### update

▸ **update**(`id`: string, `satellite`: [SatelliteType](../interfaces/satellite.satellitetype.md)): Promise\<[SatelliteType](../interfaces/satellite.satellitetype.md)>

*Defined in [src/core/satellite/satellite.update.ts:20](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/satellite/satellite.update.ts#L20)*

Update a satellite.

**`example`** 
````
friday.satellite.update(
'31f61b90-27cc-4bf6-9855-4cc59526157b',
{
  id: '31f61b90-27cc-4bf6-9855-4cc59526157b'
  name: 'satellite update'
});
````

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of satellite |
`satellite` | [SatelliteType](../interfaces/satellite.satellitetype.md) | A satellite object. |

**Returns:** Promise\<[SatelliteType](../interfaces/satellite.satellitetype.md)>

Resolve with updated satellite.
