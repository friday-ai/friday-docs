
# Plugin

- [create](#create)
- [destroy](#destroy)
- [getAll](#getAll)
- [getById](#getById)
- [update](#update)

___


{% api-method method="post" host=" " path="/api/v1/plugin" %}{% api-method-summary %}create{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to create a plugin</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %} 
{% endapi-method-headers %}

{% api-method-query-parameters %}

{% api-method-parameter name="name" type="String" required=true %}
<p>Name of the plugin.</p>{% endapi-method-parameter %}


{% api-method-parameter name="version" type="String" required=true %}
<p>Version of the plugin.</p>{% endapi-method-parameter %}


{% api-method-parameter name="url" type="String" required=true %}
<p>Url of the plugin.</p>{% endapi-method-parameter %}


{% api-method-parameter name="enabled" type="Boolean" required=false %}
<p>State of the plugin.</p>{% endapi-method-parameter %}


{% api-method-parameter name="satelliteId" type="UUIDV4" required=true %}
<p>Identifier of the satellite to which the plugin belongs.</p>{% endapi-method-parameter %}

{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  id: '33ddf1e2-3c51-4426-93af-3b0453ac0c1e',
  name: 'Zwave',
  version: '1.2.0',
  url: 'fake url',
  enabled: true,
  satelliteId: 'a7ef5f08-2bad-4489-95bf-b73fcf894d8f'
},
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host=" " path="/api/v1/plugin/:id" %}{% api-method-summary %}destroy{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to delete a plugin</p>
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

{% api-method method="get" host=" " path="/api/v1/plugin" %}{% api-method-summary %}getAll{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get all plugins</p>
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
  id: '33ddf1e2-3c51-4426-93af-3b0453ac0c1e',
  name: 'Zwave',
  version: '1.2.0',
  url: 'fake url',
  enabled: true,
  satelliteId: 'a7ef5f08-2bad-4489-95bf-b73fcf894d8f'
}],
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host=" " path="/api/v1/plugin/:if" %}{% api-method-summary %}getById{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get a plugin with his identifier</p>
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
  id: '33ddf1e2-3c51-4426-93af-3b0453ac0c1e',
  name: 'Zwave',
  version: '1.2.0',
  url: 'fake url',
  enabled: true,
  satelliteId: 'a7ef5f08-2bad-4489-95bf-b73fcf894d8f'
},
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host=" " path="/api/v1/plugin/:id" %}{% api-method-summary %}update{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to update a plugin</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %} 
{% endapi-method-headers %}

{% api-method-query-parameters %}

{% api-method-parameter name="name" type="String" required=true %}
<p>Name of the plugin.</p>{% endapi-method-parameter %}


{% api-method-parameter name="version" type="String" required=true %}
<p>Version of the plugin.</p>{% endapi-method-parameter %}


{% api-method-parameter name="url" type="String" required=true %}
<p>Url of the plugin.</p>{% endapi-method-parameter %}


{% api-method-parameter name="enabled" type="Boolean" required=false %}
<p>State of the plugin.</p>{% endapi-method-parameter %}


{% api-method-parameter name="satelliteId" type="UUIDV4" required=true %}
<p>Identifier of the satellite to which the plugin belongs.</p>{% endapi-method-parameter %}

{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  id: '33ddf1e2-3c51-4426-93af-3b0453ac0c1e',
  name: 'Zwave',
  version: '1.2.0',
  url: 'fake url',
  enabled: true,
  satelliteId: 'a7ef5f08-2bad-4489-95bf-b73fcf894d8f'
},
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}
