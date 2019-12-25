
# Scene

- [create](#create)
- [destroy](#destroy)
- [getAll](#getAll)
- [getById](#getById)

___



{% api-method method="post" host=" " path="/api/v1/scene" %}{% api-method-summary %}create{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to create an scene</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% endapi-method-headers %}

{% api-method-query-parameters %}

{% api-method-parameter name="name" type="String" required=true %}
<p>Name of the scene.</p>{% endapi-method-parameter %}


{% api-method-parameter name="description" type="String" required=false %}
<p>Description of the scene.</p>{% endapi-method-parameter %}


{% api-method-parameter name="triggerId" type="UUIDV4" required=false %}
<p>Identifier of the trigger to which the scene belongs.</p>{% endapi-method-parameter %}

{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
   id: '2452964a-a225-47dd-9b83-d88d57ed280e',
   name: 'Test scene',
   description: 'A scene for the tests ;) ',
   triggerId: 'a0f02b72-73e0-4cfd-a049-5caaa0b80514'
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="delete" host=" " path="/api/v1/scene/:id" %}{% api-method-summary %}destroy{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to delete an scene</p>
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


{% api-method method="get" host=" " path="/api/v1/scene" %}{% api-method-summary %}getAll{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get all scenes</p>
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
   id: '2452964a-a225-47dd-9b83-d88d57ed280e',
   name: 'Test scene',
   description: 'A scene for the tests ;) ',
   triggerId: 'a0f02b72-73e0-4cfd-a049-5caaa0b80514'
}]
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="get" host=" " path="/api/v1/scene/:id" %}{% api-method-summary %}getById{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get an scene with his identifier</p>
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
   id: '2452964a-a225-47dd-9b83-d88d57ed280e',
   name: 'Test scene',
   description: 'A scene for the tests ;) ',
   triggerId: 'a0f02b72-73e0-4cfd-a049-5caaa0b80514'
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}
