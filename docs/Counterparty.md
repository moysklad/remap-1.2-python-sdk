# Counterparty

Контрагент

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID контрагента | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование контрагента | [optional] 
**code** | **str** | Код контрагента | [optional] 
**external_code** | **str** | Внешний код контрагента | [optional] 
**archived** | **bool** | Добавлен ли контрагент в архив | [optional] 
**created** | **str** | Момент создания | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления | [optional] [readonly] 
**description** | **str** | Комментарий к контрагенту | [optional] 
**company_type** | **str** | Тип контрагента. Известные значения описаны в CompanyType | [optional] 
**email** | **str** | Адрес электронной почты | [optional] 
**phone** | **str** | Номер телефона | [optional] 
**fax** | **str** | Номер факса | [optional] 
**actual_address** | **str** | Фактический адрес контрагента | [optional] 
**actual_address_full** | [**Address**](Address.md) | Полный адрес | [optional] 
**legal_address** | **str** | Юридический адрес контрагента | [optional] 
**legal_address_full** | [**Address**](Address.md) | Полный юридический адрес контрагента | [optional] 
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
**birth_date** | **str** | Дата рождения для физлица | [optional] 
**sex** | **str** | Пол контрагента. Известные значения описаны в Sex | [optional] 
**discount_card_number** | **str** | Номер дисконтной карты контрагента | [optional] 
**discounts** | [**List[AgentDiscount]**](AgentDiscount.md) | Массив скидок контрагента | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) | [optional] 
**sales_amount** | **float** | Сумма продаж | [optional] [readonly] 
**bonus_points** | **int** | Бонусные баллы по активной бонусной программе | [optional] [readonly] 
**bonus_program** | [**BonusProgram**](BonusProgram.md) |  | [optional] 
**price_type** | [**PriceType**](PriceType.md) |  | [optional] 
**state** | [**State**](State.md) |  | [optional] 
**accounts** | [**CounterpartyAccounts**](CounterpartyAccounts.md) |  | [optional] 
**contactpersons** | [**CounterpartyContactpersons**](CounterpartyContactpersons.md) |  | [optional] 
**notes** | [**CounterpartyNotes**](CounterpartyNotes.md) |  | [optional] 
**files** | [**FileList**](FileList.md) |  | [optional] 
**tags** | **List[str]** | Группы контрагента | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Дополнительные поля | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.counterparty import Counterparty

# TODO update the JSON string below
json = "{}"
# create an instance of Counterparty from a JSON string
counterparty_instance = Counterparty.from_json(json)
# print the JSON string representation of the object
print(Counterparty.to_json())

# convert the object into a dict
counterparty_dict = counterparty_instance.to_dict()
# create an instance of Counterparty from a dict
counterparty_from_dict = Counterparty.from_dict(counterparty_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


