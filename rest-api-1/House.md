
# House

- [create](#create)
- [destroy](#destroy)
- [getAll](#getAll)
- [getById](#getById)
- [update](#update)

___


{% api-method method="post" host=" " path="/api/v1/house" %}{% api-method-summary %}create{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to create an house</p>
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


{% api-method-parameter name="latitude" type="String" required=true %}
<p>Latitude of the house.</p>{% endapi-method-parameter %}


{% api-method-parameter name="longitude" type="String" required=true %}
<p>Longitude of the house.</p>{% endapi-method-parameter %}

{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  id: 'ecb7958f-ea9e-4520-819e-be6358dc407c',
  name: 'Main House',
  latitude: '34.0012295',
  longitude: '-118.8067245'
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host=" " path="/api/v1/house/:id" %}{% api-method-summary %}destroy{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to delete an house</p>
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

{% api-method method="get" host=" " path="/api/v1/house" %}{% api-method-summary %}getAll{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get all houses</p>
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
  id: 'ecb7958f-ea9e-4520-819e-be6358dc407c',
  name: 'Main House',
  latitude: '34.0012295',
  longitude: '-118.8067245'
}]
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host=" " path="/api/v1/house/:id" %}{% api-method-summary %}getById{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get an house with his identifier</p>
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
  id: 'ecb7958f-ea9e-4520-819e-be6358dc407c',
  name: 'Main House',
  latitude: '34.0012295',
  longitude: '-118.8067245'
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="patch" host=" " path="/api/v1/house/:id" %}{% api-method-summary %}update{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to update an house</p>
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


{% api-method-parameter name="latitude" type="String" required=true %}
<p>Latitude of the house.</p>{% endapi-method-parameter %}


{% api-method-parameter name="longitude" type="String" required=true %}
<p>Longitude of the house.</p>{% endapi-method-parameter %}

{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  id: 'ecb7958f-ea9e-4520-819e-be6358dc407c',
  name: 'Main House',
  latitude: '34.0012295',
  longitude: '-118.8067245'
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}
