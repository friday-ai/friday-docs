> **[friday-server](../README.md)**

[Globals](../globals.md) / [device](device.md) /

# External module: device

### Index

#### Classes

* [Device](../classes/device.device-1.md)

#### Interfaces

* [DeviceType](../interfaces/device.devicetype.md)

#### Functions

* [create](device.md#create)
* [destroy](device.md#destroy)
* [getAll](device.md#getall)
* [getById](device.md#getbyid)
* [update](device.md#update)

## Functions

###  create

▸ **create**(`device`: [DeviceType](../interfaces/device.devicetype.md)): *`Promise<DeviceType>`*

Defined in device/device.create.ts:25

Create a device.

**`example`** 
````
friday.device.create({
   id: '8ae2dc77-a733-45b9-bbe6-69d837222dce',
   name: 'Light sample',
   type: AvailableTypeOfDevice.LIGHT,
   subType: AvailableSubTypeOfDevice.LIGHT_RGB,
   variable: '',
   unit: '',
   value: 'on',
   roomId: '84901b92-06fe-4f0f-93bd-d4ead2105720',
   pluginId: ''
});
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`device` | [DeviceType](../interfaces/device.devicetype.md) | A device object. |

**Returns:** *`Promise<DeviceType>`*

Resolve with created device.

___

###  destroy

▸ **destroy**(`id`: string): *`Promise<void>`*

Defined in device/device.destroy.ts:14

Destroy a device.

**`example`** 
````
friday.device.destroy('ffba6936-2ce0-411c-91c9-6f1dd6ed0b17');
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of device. |

**Returns:** *`Promise<void>`*

___

###  getAll

▸ **getAll**(`options?`: `GetOptions`): *`Promise<DeviceType[]>`*

Defined in device/device.getAll.ts:26

Get all devices.

**`example`** 
````
friday.device.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`options?` | `GetOptions` | Options of the query. |

**Returns:** *`Promise<DeviceType[]>`*

Resolve with device array.

___

###  getById

▸ **getById**(`id`: string, `scope?`: undefined | string): *`Promise<DeviceType>`*

Defined in device/device.getById.ts:16

Get a device by id.

**`example`** 
````
friday.device.getById('40085fb8-1784-49be-84ad-8adbca1ebc3d', 'full');
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`id` | string | Id of device. |
`scope?` | undefined \| string | Scope option. (Optional) |

**Returns:** *`Promise<DeviceType>`*

Resolve with device.

___

###  update

▸ **update**(`device`: [DeviceType](../interfaces/device.devicetype.md)): *`Promise<DeviceType>`*

Defined in device/device.update.ts:18

Update a device.

**`example`** 
````
friday.device.update({
  id: '36440e00-bef2-4cdb-883e-1bada5bc501b'
  name: 'device update'
});
````

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`device` | [DeviceType](../interfaces/device.devicetype.md) | A device object. |

**Returns:** *`Promise<DeviceType>`*

Resolve with updated device.