# Organization

Юрлицо

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID юрлица | [optional] [readonly] 
**sync_id** | **str** | ID синхронизации | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование юрлица | [optional] 
**code** | **str** | Код юрлица | [optional] 
**external_code** | **str** | Внешний код юрлица | [optional] 
**archived** | **bool** | Добавлено ли юрлицо в архив | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления юрлица | [optional] [readonly] 
**description** | **str** | Комментарий к юрлицу | [optional] 
**company_type** | **str** | Тип юрлица. Известные значения описаны в CompanyType | [optional] 
**email** | **str** | Адрес электронной почты | [optional] 
**phone** | **str** | Номер городского телефона | [optional] 
**fax** | **str** | Номер факса | [optional] 
**actual_address** | **str** | Фактический адрес юрлица | [optional] 
**actual_address_full** | [**Address**](Address.md) | Фактический адрес юрлица с детализацией по отдельным полям | [optional] 
**legal_address** | **str** | Юридический адрес юрлица | [optional] 
**legal_address_full** | [**Address**](Address.md) | Юридический адрес юрлица с детализацией по отдельным полям | [optional] 
**inn** | **str** | ИНН | [optional] 
**kpp** | **str** | КПП | [optional] 
**ogrn** | **str** | ОГРН | [optional] 
**ogrnip** | **str** | ОГРНИП | [optional] 
**okpo** | **str** | ОКПО | [optional] 
**certificate_number** | **str** | Номер свидетельства | [optional] 
**certificate_date** | **str** | Дата свидетельства | [optional] 
**legal_title** | **str** | Полное наименование | [optional] 
**legal_first_name** | **str** | Имя для ИП и физлица | [optional] 
**legal_last_name** | **str** | Фамилия для ИП и физлица | [optional] 
**legal_middle_name** | **str** | Отчество для ИП и физлица | [optional] 
**tracking_contract_number** | **str** | Номер договора с ЦРПТ | [optional] 
**tracking_contract_date** | **str** | Дата договора с ЦРПТ | [optional] 
**advance_payment_vat** | **float** | Налоговая ставка для авансов для плательщиков НДС | [optional] 
**payer_vat** | **bool** | Является ли данное юрлицо плательщиком НДС | [optional] 
**director** | **str** | Руководитель | [optional] 
**director_position** | **str** | Должность руководителя | [optional] 
**chief_accountant** | **str** | Главный бухгалтер | [optional] 
**director_sign** | [**Image**](Image.md) | Подпись руководителя | [optional] 
**chief_account_sign** | [**Image**](Image.md) | Подпись главного бухгалтера | [optional] 
**stamp** | [**Image**](Image.md) | Печать | [optional] 
**bonus_points** | **int** | Бонусные баллы по активной бонусной программе | [optional] [readonly] 
**bonus_program** | [**BonusProgram**](BonusProgram.md) | Метаданные активной бонусной программы | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) | [optional] 
**accounts** | [**OrganizationAccounts**](OrganizationAccounts.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Дополнительные поля | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.organization import Organization

# TODO update the JSON string below
json = "{}"
# create an instance of Organization from a JSON string
organization_instance = Organization.from_json(json)
# print the JSON string representation of the object
print(Organization.to_json())

# convert the object into a dict
organization_dict = organization_instance.to_dict()
# create an instance of Organization from a dict
organization_from_dict = Organization.from_dict(organization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


