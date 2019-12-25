
# Room

- [create](#create)
- [destroy](#destroy)
- [getAll](#getAll)
- [getById](#getById)

___



{% api-method method="patch" host=" " path="/api/v1/room" %}{% api-method-summary %}create{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to update an room</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% endapi-method-headers %}

{% api-method-query-parameters %}

{% api-method-parameter name="name" type="String" required=true %}
<p>Name of the house.</p>{% endapi-method-parameter %}


{% api-method-parameter name="houseId" type="UUIDV4" required=true %}
<p>Identifier of the house to which the room belongs.</p>{% endapi-method-parameter %}

{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  id: 'c97ba085-ba97-4a30-bdd3-b7a62f6514dc',
  name: 'Bedroom',
  houseId: 'ecb7958f-ea9e-4520-819e-be6358dc407c'
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="delete" host=" " path="/api/v1/room/:id" %}{% api-method-summary %}destroy{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to delete an room</p>
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


{% api-method method="get" host=" " path="/api/v1/room" %}{% api-method-summary %}getAll{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get all rooms</p>
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
  id: 'c97ba085-ba97-4a30-bdd3-b7a62f6514dc',
  name: 'Bedroom',
  houseId: 'ecb7958f-ea9e-4520-819e-be6358dc407c'
}]
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="get" host=" " path="/api/v1/room/:id" %}{% api-method-summary %}getById{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get an room with his identifier</p>
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
  id: 'c97ba085-ba97-4a30-bdd3-b7a62f6514dc',
  name: 'Bedroom',
  houseId: 'ecb7958f-ea9e-4520-819e-be6358dc407c'
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}
