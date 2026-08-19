# UserSettings

Настройки пользователя

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**auto_show_reports** | **bool** | Строить ли отчеты автоматически при переходе на вкладку с отчетом | [optional] 
**default_company** | [**Organization**](Organization.md) |  | [optional] 
**default_customer_counterparty** | [**Counterparty**](Counterparty.md) |  | [optional] 
**default_place** | [**Store**](Store.md) |  | [optional] 
**default_project** | [**Project**](Project.md) |  | [optional] 
**default_purchase_counterparty** | [**Counterparty**](Counterparty.md) |  | [optional] 
**default_screen** | **str** | Стартовый экран пользователя. Известные значения описаны в DefaultScreen | [optional] 
**fields_per_row** | **int** | Количество столбцов, в которых будут располагаться дополнительные поля в документах | [optional] 
**locale** | **str** | Язык системы. Известные значения описаны в Locale | [optional] 
**mail_footer** | **str** | Подставляется в подпись в письмах, отправляемых из МС | [optional] 
**print_format** | **str** | Правила печати документов. Известные значения описаны в PrintFormat | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.user_settings import UserSettings

# TODO update the JSON string below
json = "{}"
# create an instance of UserSettings from a JSON string
user_settings_instance = UserSettings.from_json(json)
# print the JSON string representation of the object
print(UserSettings.to_json())

# convert the object into a dict
user_settings_dict = user_settings_instance.to_dict()
# create an instance of UserSettings from a dict
user_settings_from_dict = UserSettings.from_dict(user_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


