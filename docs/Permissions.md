# Permissions

Права на сущность. BASE включает view, create, update и delete; DICTIONARY дополнительно включает print; OPERATION — print и approve. Для GTINList используются view, create и delete, для trackingCodeList — view и print. Известные значения описаны в PermissionValue. Область действия расширяется по цепочкам NO → OWN → OWN_SHARED → OWN_GROUP_SHARED → ALL и NO → OWN → OWN_GROUP → OWN_GROUP_SHARED → ALL. Неуказанное действие запрещено сотруднику. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**view** | **str** | Смотреть. Известные значения описаны в PermissionValue. | [optional] 
**var_print** | **str** | Печатать. Известные значения описаны в PermissionValue. Значение совпадает с view или отсутствует. | [optional] 
**create** | **str** | Создавать. Известные значения описаны в PermissionValue. Значение совпадает с view или отсутствует. | [optional] 
**update** | **str** | Редактировать. Известные значения описаны в PermissionValue. Область действия не шире view; поле может отсутствовать. | [optional] 
**delete** | **str** | Удалять. Известные значения описаны в PermissionValue. Значение совпадает с update или отсутствует. | [optional] 
**approve** | **str** | Проводить. Известные значения описаны в PermissionValue. Значение совпадает с view или отсутствует. | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.permissions import Permissions

# TODO update the JSON string below
json = "{}"
# create an instance of Permissions from a JSON string
permissions_instance = Permissions.from_json(json)
# print the JSON string representation of the object
print(Permissions.to_json())

# convert the object into a dict
permissions_dict = permissions_instance.to_dict()
# create an instance of Permissions from a dict
permissions_from_dict = Permissions.from_dict(permissions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


