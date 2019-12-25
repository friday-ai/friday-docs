
# Action

- [create](#create)
- [destroy](#destroy)
- [getAll](#getAll)
- [getById](#getById)
- [update](#update)

___



{% api-method method="post" host=" " path="/api/v1/action" %}{% api-method-summary %}create{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to create an action</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% endapi-method-headers %}

{% api-method-query-parameters %}

{% api-method-parameter name="name" type="String" required=true %}
<p>Name of the action.</p>{% endapi-method-parameter %}


{% api-method-parameter name="description" type="String" required=false %}
<p>Description of the action.</p>{% endapi-method-parameter %}


{% api-method-parameter name="type" type="ActionsType" required=true %}
<p>Type of the action.</p>{% endapi-method-parameter %}


{% api-method-parameter name="subType" type="String" required=true %}
<p>SubType of the action.</p>{% endapi-method-parameter %}


{% api-method-parameter name="variableKey" type="String" required=true %}
<p>Name of the object affected by the action.</p>{% endapi-method-parameter %}


{% api-method-parameter name="variable" type="String" required=true %}
<p>Value Value to give to the object affected by the action.</p>{% endapi-method-parameter %}


{% api-method-parameter name="sceneId" type="UUIDV4" required=true %}
<p>Identifier of the scene to which the action belongs.</p>{% endapi-method-parameter %}

{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  "id": "daff2ca0-5ab8-4e72-8561-c4ed9c7c6901",
  "name": "action example",
  "description": "action example description",
  "type": "light.turn_on",
  "subType": "",
  "variableKey": "action example variable key",
  "variableValue": "action example variable value",
  "sceneId": "2452964a-a225-47dd-9b83-d88d57ed280e"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="delete" host=" " path="/api/v1/action/:id" %}{% api-method-summary %}destroy{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to delete an action</p>
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


{% api-method method="get" host=" " path="/api/v1/action" %}{% api-method-summary %}getAll{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get all actions</p>
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
  "id": "daff2ca0-5ab8-4e72-8561-c4ed9c7c6901",
  "name": "action example",
  "description": "action example description",
  "type": "light.turn_on",
  "subType": "",
  "variableKey": "action example variable key",
  "variableValue": "action example variable value",
  "sceneId": "2452964a-a225-47dd-9b83-d88d57ed280e"
}]
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="get" host=" " path="/api/v1/action/:id" %}{% api-method-summary %}getById{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get an action with his identifier</p>
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
  "id": "daff2ca0-5ab8-4e72-8561-c4ed9c7c6901",
  "name": "action example",
  "description": "action example description",
  "type": "light.turn_on",
  "subType": "",
  "variableKey": "action example variable key",
  "variableValue": "action example variable value",
  "sceneId": "2452964a-a225-47dd-9b83-d88d57ed280e"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="patch" host=" " path="/api/v1/action/:id" %}{% api-method-summary %}update{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to update an action</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% endapi-method-headers %}

{% api-method-query-parameters %}

{% api-method-parameter name="name" type="String" required=true %}
<p>Name of the action.</p>{% endapi-method-parameter %}


{% api-method-parameter name="description" type="String" required=false %}
<p>Description of the action.</p>{% endapi-method-parameter %}


{% api-method-parameter name="type" type="ActionsType" required=true %}
<p>Type of the action.</p>{% endapi-method-parameter %}


{% api-method-parameter name="subType" type="String" required=true %}
<p>SubType of the action.</p>{% endapi-method-parameter %}


{% api-method-parameter name="variableKey" type="String" required=true %}
<p>Name of the object affected by the action.</p>{% endapi-method-parameter %}


{% api-method-parameter name="variable" type="String" required=true %}
<p>Value Value to give to the object affected by the action.</p>{% endapi-method-parameter %}


{% api-method-parameter name="sceneId" type="UUIDV4" required=true %}
<p>Identifier of the scene to which the action belongs.</p>{% endapi-method-parameter %}

{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  "id": "daff2ca0-5ab8-4e72-8561-c4ed9c7c6901",
  "name": "action example",
  "description": "action example description",
  "type": "light.turn_on",
  "subType": "",
  "variableKey": "action example variable key",
  "variableValue": "action example variable value",
  "sceneId": "2452964a-a225-47dd-9b83-d88d57ed280e"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}
