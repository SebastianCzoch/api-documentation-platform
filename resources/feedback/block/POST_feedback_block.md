# Feedback Block Resources
    POST feedback/:feedback_id/block

## Description
Create a feedback block

## Requires authentication
- Details described [here](/README.md#authentication)

## Parameters
- `category` _(required)_ - feedback category ([reference](/reference/feedback/block/category.md))
- `type` _(required)_ - feedback block type, either `string` or `non-textual`
- `ridx` _(required)_ - for type `non-textual`, id marked on screenshot
- `string`_(required)_ - for type `string`, feedback string
- `comment`_(optional)_ - comment on feedback block
- `suggestion`_(optional)_ - suggestion on feedback
- `translated_string` _(optional) - translated string id in platform to associated with

## Example
**Request**

    POST https://api.platform.onesky.io/1/feedback/:feedback_id/block

**Response**
```
status 201 Created
```