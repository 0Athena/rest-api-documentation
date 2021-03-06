# Contact Custom Field List

    GET services/:service_id/contact-custom-fields
    
Returns a list of [Contact Custom Fields]  belonging to the specified service




## Parameters
### URI Parameters
Field | Wildcards | Description
--- | --- | ---
Pagination options | N | (see [Overview - Request Modifiers][])
### Sortable fields
* id
* data_type

## Example
### Request

    GET https://api.zingle.me/v1/services/aff8bc93-6e28-4e70-8770-defa35cdfc1b/contact-custom-fields

### Response
``` json
{
    "status": {
        "text": "OK",
        "status_code": 200,
        "description": null,
        "sort_field": "id",
        "sort_direction": "asc",
        "page": 1,
        "page_size": 10,
        "total_pages": 1,
        "total_records": 4
    },
    "result": [
        {
          "id": "56c70519-6c70-40e5-904e-7652e54a07b6",
          "display_name": "First Name",
          "code": "first_name",
          "data_type": "string",
          "replacement_variable": "FIRST NAME",
          "is_global": true,
          "options": []
        },
        {
          "id": "29fdae7d-c5d7-4cd6-b2e4-cd52603ff577",
          "display_name": "Last Name",
          "code": "last_name",          
          "data_type": "string",
          "replacement_variable": "LAST NAME",
          "is_global": true,
          "options": []
        },    
        {
          "id": "7f6318f4-14ea-4f8c-bde4-c76ed704060a",
          "display_name": "Checkin Date",
          "code": "checkin_date",          
          "data_type": "date",
          "replacement_variable": "CHECKIN DATE",
          "is_global": true,
          "options": []
        },
        {
          "id": "fc12db04-66b1-416a-83d4-8532e344737f",
          "display_name": "Checkout Date",
          "code": "checkout_date",          
          "data_type": "date",
          "replacement_variable": "CHECKOUT DATE",
          "is_global": true,
          "options": []
        }     
    ]
}
```

[Overview - Request Modifiers]: /README.md#request-modifiers
[Contact Custom Fields]: README.md
