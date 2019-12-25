
# Device

- [create](#create)
- [destroy](#destroy)
- [getAll](#getAll)
- [getById](#getById)
- [update](#update)

___



{% api-method method="post" host=" " path="/api/v1/device" %}{% api-method-summary %}create{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to create a device</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% endapi-method-headers %}

{% api-method-query-parameters %}

{% api-method-parameter name="name" type="String" required=true %}
<p>Name of the device.</p>{% endapi-method-parameter %}


{% api-method-parameter name="type" type="AvailableTypeOfDevice" required=true %}
<p>Type of the device.</p>{% endapi-method-parameter %}


{% api-method-parameter name="subType" type="AvailableSubTypeOfDevice" required=true %}
<p>Subtype of the device.</p>{% endapi-method-parameter %}


{% api-method-parameter name="variable" type="Any" required=false %}
<p>Variable attached of device.</p>{% endapi-method-parameter %}


{% api-method-parameter name="unit" type="String" required=false %}
<p>Unit of device.</p>{% endapi-method-parameter %}


{% api-method-parameter name="value" type="String" required=false %}
<p>Value of device.</p>{% endapi-method-parameter %}


{% api-method-parameter name="roomId" type="UUIDV4" required=true %}
<p>Identifier of the room to which the device belongs.</p>{% endapi-method-parameter %}


{% api-method-parameter name="pluginId" type="UUIDV4" required=true %}
<p>Plugin of the scene to which the device belongs.</p>{% endapi-method-parameter %}

{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  id: '22b5b9ce-cd9e-404a-8c31-97350d684fd3',
  name: 'Light',
  type: AvailableTypeOfDevice.LIGHT,
  subType: AvailableSubTypeOfDevice.LIGHT_RGB,
  variable: '',
  unit: '',
  value: 'on',
  roomId: 'c97ba085-ba97-4a30-bdd3-b7a62f6514dc',
  pluginId: '33ddf1e2-3c51-4426-93af-3b0453ac0c1e'
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="delete" host=" " path="/api/v1/device/:id" %}{% api-method-summary %}destroy{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to delete a device</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  "success": "true",
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="get" host=" " path="/api/v1/device" %}{% api-method-summary %}getAll{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get all devices</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
[{
  id: '22b5b9ce-cd9e-404a-8c31-97350d684fd3',
  name: 'Light',
  type: AvailableTypeOfDevice.LIGHT,
  subType: AvailableSubTypeOfDevice.LIGHT_RGB,
  variable: '',
  unit: '',
  value: 'on',
  roomId: 'c97ba085-ba97-4a30-bdd3-b7a62f6514dc',
  pluginId: '33ddf1e2-3c51-4426-93af-3b0453ac0c1e'
}]
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="get" host=" " path="/api/v1/device/:id" %}{% api-method-summary %}getById{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get a device with his identifier</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  id: '22b5b9ce-cd9e-404a-8c31-97350d684fd3',
  name: 'Light',
  type: AvailableTypeOfDevice.LIGHT,
  subType: AvailableSubTypeOfDevice.LIGHT_RGB,
  variable: '',
  unit: '',
  value: 'on',
  roomId: 'c97ba085-ba97-4a30-bdd3-b7a62f6514dc',
  pluginId: '33ddf1e2-3c51-4426-93af-3b0453ac0c1e'
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="patch" host=" " path="/api/v1/device/:id" %}{% api-method-summary %}update{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to update a device</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% endapi-method-headers %}

{% api-method-query-parameters %}

{% api-method-parameter name="name" type="String" required=true %}
<p>Name of the device.</p>{% endapi-method-parameter %}


{% api-method-parameter name="type" type="AvailableTypeOfDevice" required=true %}
<p>Type of the device.</p>{% endapi-method-parameter %}


{% api-method-parameter name="subType" type="AvailableSubTypeOfDevice" required=true %}
<p>Subtype of the device.</p>{% endapi-method-parameter %}


{% api-method-parameter name="variable" type="Any" required=false %}
<p>Variable attached of device.</p>{% endapi-method-parameter %}


{% api-method-parameter name="unit" type="String" required=false %}
<p>Unit of device.</p>{% endapi-method-parameter %}


{% api-method-parameter name="value" type="String" required=false %}
<p>Value of device.</p>{% endapi-method-parameter %}


{% api-method-parameter name="roomId" type="UUIDV4" required=true %}
<p>Identifier of the room to which the device belongs.</p>{% endapi-method-parameter %}


{% api-method-parameter name="pluginId" type="UUIDV4" required=true %}
<p>Plugin of the scene to which the device belongs.</p>{% endapi-method-parameter %}

{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  id: '22b5b9ce-cd9e-404a-8c31-97350d684fd3',
  name: 'Light',
  type: AvailableTypeOfDevice.LIGHT,
  subType: AvailableSubTypeOfDevice.LIGHT_RGB,
  variable: '',
  unit: '',
  value: 'on',
  roomId: 'c97ba085-ba97-4a30-bdd3-b7a62f6514dc',
  pluginId: '33ddf1e2-3c51-4426-93af-3b0453ac0c1e'
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}
