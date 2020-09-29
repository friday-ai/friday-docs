**friday-server**

> [README](../README.md) / [Globals](../globals.md) / [state](../modules/state.md) / StateType

# Interface: StateType

State interface.

## Hierarchy

* **StateType**

## Index

### Properties

* [device](state.statetype.md#device)
* [house](state.statetype.md#house)
* [id](state.statetype.md#id)
* [last](state.statetype.md#last)
* [owner](state.statetype.md#owner)
* [ownerType](state.statetype.md#ownertype)
* [plugin](state.statetype.md#plugin)
* [room](state.statetype.md#room)
* [satellite](state.statetype.md#satellite)
* [user](state.statetype.md#user)
* [value](state.statetype.md#value)

## Properties

### device

• `Optional` **device**: [DeviceType](device.devicetype.md)

*Defined in [src/core/state/state.interface.ts:23](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/state/state.interface.ts#L23)*

___

### house

• `Optional` **house**: [HouseType](house.housetype.md)

*Defined in [src/core/state/state.interface.ts:20](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/state/state.interface.ts#L20)*

___

### id

• `Optional` **id**: undefined \| string

*Defined in [src/core/state/state.interface.ts:13](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/state/state.interface.ts#L13)*

___

### last

• `Optional` **last**: undefined \| false \| true

*Defined in [src/core/state/state.interface.ts:17](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/state/state.interface.ts#L17)*

___

### owner

•  **owner**: string

*Defined in [src/core/state/state.interface.ts:14](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/state/state.interface.ts#L14)*

___

### ownerType

•  **ownerType**: StateOwner

*Defined in [src/core/state/state.interface.ts:15](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/state/state.interface.ts#L15)*

___

### plugin

• `Optional` **plugin**: [PluginType](plugin.plugintype.md)

*Defined in [src/core/state/state.interface.ts:21](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/state/state.interface.ts#L21)*

___

### room

• `Optional` **room**: [RoomType](room.roomtype.md)

*Defined in [src/core/state/state.interface.ts:19](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/state/state.interface.ts#L19)*

___

### satellite

• `Optional` **satellite**: [SatelliteType](satellite.satellitetype.md)

*Defined in [src/core/state/state.interface.ts:22](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/state/state.interface.ts#L22)*

___

### user

• `Optional` **user**: [UserType](user.usertype.md)

*Defined in [src/core/state/state.interface.ts:18](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/state/state.interface.ts#L18)*

___

### value

•  **value**: AvailableState

*Defined in [src/core/state/state.interface.ts:16](https://github.com/friday-ai/friday/blob/cd1d9b5/server/src/core/state/state.interface.ts#L16)*
