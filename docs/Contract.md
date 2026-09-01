# Contract

Договор

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Договора | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Номер договора | [optional] 
**description** | **str** | Описание Договора | [optional] 
**code** | **str** | Код Договора | [optional] 
**external_code** | **str** | Внешний код Договора | [optional] 
**archived** | **bool** | Добавлен ли Договор в архив | [optional] 
**moment** | **str** | Дата Договора | [optional] 
**sum** | **int** | Сумма Договора | [optional] 
**contract_type** | **str** | Тип Договора. Известные значения описаны в ContractType | [optional] 
**reward_type** | **str** | Тип Вознаграждения. Известные значения описаны в RewardType | [optional] 
**reward_percent** | **float** | Вознаграждение в процентах (от 0 до 100) | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления сущности | [optional] [readonly] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**own_agent** | [**Organization**](Organization.md) |  | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица | [optional] 
**state** | [**State**](State.md) | Метаданные статуса договора | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета вашего юрлица | [optional] 
**agent_account** | [**Account**](Account.md) | Метаданные счета контрагента | [optional] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция доп. полей | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.contract import Contract

# TODO update the JSON string below
json = "{}"
# create an instance of Contract from a JSON string
contract_instance = Contract.from_json(json)
# print the JSON string representation of the object
print(Contract.to_json())

# convert the object into a dict
contract_dict = contract_instance.to_dict()
# create an instance of Contract from a dict
contract_from_dict = Contract.from_dict(contract_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


