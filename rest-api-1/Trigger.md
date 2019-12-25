
# Trigger

- [create](#create)
- [destroy](#destroy)
- [getAll](#getAll)
- [getById](#getById)

___



{% api-method method="post" host=" " path="/api/v1/trigger" %}{% api-method-summary %}create{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to create a trigger</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% endapi-method-headers %}

{% api-method-query-parameters %}

{% api-method-parameter name="name" type="String" required=true %}
<p>Name of the trigger.</p>{% endapi-method-parameter %}


{% api-method-parameter name="description" type="String" required=false %}
<p>Description of the trigger.</p>{% endapi-method-parameter %}


{% api-method-parameter name="type" type="AvailableConditions" required=true %}
<p>Type of the trigger.</p>{% endapi-method-parameter %}


{% api-method-parameter name="rules" type="JSON" required=true %}
<p>Rules of the trigger.</p>{% endapi-method-parameter %}

{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  id: 'a0f02b72-73e0-4cfd-a049-5caaa0b80514',
  name: 'Test',
  description: 'A trigger test',
  type: 'device.value',
  rules: {
    device: 'cc306435-eb0f-455c-b79d-a684b171e04d',
    value: '23'
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="delete" host=" " path="/api/v1/trigger/:id" %}{% api-method-summary %}destroy{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to delete a trigger</p>
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


{% api-method method="get" host=" " path="/api/v1/trigger" %}{% api-method-summary %}getAll{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get all triggers</p>
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
  id: 'a0f02b72-73e0-4cfd-a049-5caaa0b80514',
  name: 'Test',
  description: 'A trigger test',
  type: 'device.value',
  rules: {
    device: 'cc306435-eb0f-455c-b79d-a684b171e04d',
    value: '23'
  }
}]
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="get" host=" " path="/api/v1/trigger/:id" %}{% api-method-summary %}getById{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get a trigger with his identifier</p>
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
  id: 'a0f02b72-73e0-4cfd-a049-5caaa0b80514',
  name: 'Test',
  description: 'A trigger test',
  type: 'device.value',
  rules: {
    device: 'cc306435-eb0f-455c-b79d-a684b171e04d',
    value: '23'
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}
