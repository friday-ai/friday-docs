# device

> [**friday-server**](./)

[Globals](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/globals.md) / [device](device.md) /

## External module: device

#### Index

**Classes**

* [Device](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/classes/device.device-1.md)

**Interfaces**

* [DeviceType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/device.devicetype.md)

**Functions**

* [create](device.md#create)
* [destroy](device.md#destroy)
* [getAll](device.md#getall)
* [getById](device.md#getbyid)
* [update](device.md#update)

### Functions

#### create

▸ **create**\(`device`: [DeviceType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/device.devicetype.md)\): _`Promise<DeviceType>`_

Defined in device/device.create.ts:25

Create a device.

**`example`**

```text
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
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `device` | [DeviceType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/device.devicetype.md) | A device object. |

**Returns:** _`Promise<DeviceType>`_

Resolve with created device.

#### destroy

▸ **destroy**\(`id`: string\): _`Promise<void>`_

Defined in device/device.destroy.ts:14

Destroy a device.

**`example`**

```text
friday.device.destroy('ffba6936-2ce0-411c-91c9-6f1dd6ed0b17');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `id` | string | Id of device. |

**Returns:** _`Promise<void>`_

#### getAll

▸ **getAll**\(`options?`: `GetOptions`\): _`Promise<DeviceType[]>`_

Defined in device/device.getAll.ts:26

Get all devices.

**`example`**

```text
friday.device.getAll({
   scope: '',
   take: 20,
   skip: 0
 });
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `options?` | `GetOptions` | Options of the query. |

**Returns:** _`Promise<DeviceType[]>`_

Resolve with device array.

#### getById

▸ **getById**\(`id`: string, `scope?`: undefined \| string\): _`Promise<DeviceType>`_

Defined in device/device.getById.ts:16

Get a device by id.

**`example`**

```text
friday.device.getById('40085fb8-1784-49be-84ad-8adbca1ebc3d', 'full');
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `id` | string | Id of device. |
| `scope?` | undefined \| string | Scope option. \(Optional\) |

**Returns:** _`Promise<DeviceType>`_

Resolve with device.

#### update

▸ **update**\(`device`: [DeviceType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/device.devicetype.md)\): _`Promise<DeviceType>`_

Defined in device/device.update.ts:18

Update a device.

**`example`**

```text
friday.device.update({
  id: '36440e00-bef2-4cdb-883e-1bada5bc501b'
  name: 'device update'
});
```

**Parameters:**

| Name | Type | Description |
| :--- | :--- | :--- |
| `device` | [DeviceType](https://github.com/friday-ai/friday-docs/tree/7469fd0637aa28a674d6c68645188ee863701e30/node-js-api-1/interfaces/device.devicetype.md) | A device object. |

**Returns:** _`Promise<DeviceType>`_

Resolve with updated device.

