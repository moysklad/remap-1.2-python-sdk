# ContactPerson

Контактные лица Контрагентов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID контактного лица | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**updated** | **str** | Время последнего изменения | [optional] [readonly] 
**name** | **str** | ФИО контактного лица | [optional] 
**description** | **str** | Описание контактного лица | [optional] 
**email** | **str** | Адрес электронной почты | [optional] 
**phone** | **str** | Номер телефона | [optional] 
**position** | **str** | Должность | [optional] 
**external_code** | **str** | Внешний код контактного лица | [optional] 
**agent** | [**Counterparty**](Counterparty.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.contact_person import ContactPerson

# TODO update the JSON string below
json = "{}"
# create an instance of ContactPerson from a JSON string
contact_person_instance = ContactPerson.from_json(json)
# print the JSON string representation of the object
print(ContactPerson.to_json())

# convert the object into a dict
contact_person_dict = contact_person_instance.to_dict()
# create an instance of ContactPerson from a dict
contact_person_from_dict = ContactPerson.from_dict(contact_person_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


