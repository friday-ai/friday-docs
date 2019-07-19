> **[friday-server](../README.md)**

[Globals](../globals.md) / [state](../modules/state.md) / [StateType](state.statetype.md) /

# Interface: StateType

State interface.

## Hierarchy

* **StateType**

### Index

#### Properties

* [device](state.statetype.md#optional-device)
* [house](state.statetype.md#optional-house)
* [id](state.statetype.md#id)
* [owner](state.statetype.md#owner)
* [ownerType](state.statetype.md#ownertype)
* [plugin](state.statetype.md#optional-plugin)
* [room](state.statetype.md#optional-room)
* [satellite](state.statetype.md#optional-satellite)
* [user](state.statetype.md#optional-user)
* [value](state.statetype.md#value)

## Properties

### `Optional` device

• **device**? : *[DeviceType](device.devicetype.md)*

Defined in state/state.interface.ts:22

___

### `Optional` house

• **house**? : *[HouseType](house.housetype.md)*

Defined in state/state.interface.ts:19

___

###  id

• **id**: *string*

Defined in state/state.interface.ts:13

___

###  owner

• **owner**: *string*

Defined in state/state.interface.ts:14

___

###  ownerType

• **ownerType**: *`StateOwner`*

Defined in state/state.interface.ts:15

___

### `Optional` plugin

• **plugin**? : *[PluginType](plugin.plugintype.md)*

Defined in state/state.interface.ts:20

___

### `Optional` room

• **room**? : *[RoomType](room.roomtype.md)*

Defined in state/state.interface.ts:18

___

### `Optional` satellite

• **satellite**? : *[SatelliteType](satellite.satellitetype.md)*

Defined in state/state.interface.ts:21

___

### `Optional` user

• **user**? : *[UserType](user.usertype.md)*

Defined in state/state.interface.ts:17

___

###  value

• **value**: *`AvailableState`*

Defined in state/state.interface.ts:16