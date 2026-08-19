# BonusTransaction

Бонусная операция (bonustransaction)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID бонусной операции | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**owner** | [**Employee**](Employee.md) |  | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица, связанного с бонусной операцией | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**parent_document** | [**BonusTransactionParentDocument**](BonusTransactionParentDocument.md) |  | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**bonus_program** | [**BonusProgram**](BonusProgram.md) |  | [optional] 
**bonus_value** | **int** | Количество бонусных баллов | [optional] 
**transaction_type** | **str** | Тип бонусной операции. Известные значения описаны в TransactionType | [optional] 
**transaction_status** | **str** | Статус бонусной операции. Известные значения описаны в TransactionStatus | [optional] [readonly] 
**category_type** | **str** | Категория бонусной операции. Известные значения описаны в CategoryType | [optional] [readonly] 
**code** | **str** | Код бонусной операции | [optional] 
**name** | **str** | Наименование бонусной операции | [optional] 
**external_code** | **str** | Внешний код бонусной операции | [optional] 
**description** | **str** | Комментарий к бонусной операции | [optional] 
**moment** | **str** | Время проведения бонусной операции | [optional] 
**created** | **str** | Момент создания бонусной операции | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления бонусной операции | [optional] [readonly] 
**execution_date** | **str** | Дата начисления бонусной операции | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**updated_by** | **str** | Автор последнего обновления (uid, используется для фильтрации) | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.bonus_transaction import BonusTransaction

# TODO update the JSON string below
json = "{}"
# create an instance of BonusTransaction from a JSON string
bonus_transaction_instance = BonusTransaction.from_json(json)
# print the JSON string representation of the object
print(BonusTransaction.to_json())

# convert the object into a dict
bonus_transaction_dict = bonus_transaction_instance.to_dict()
# create an instance of BonusTransaction from a dict
bonus_transaction_from_dict = BonusTransaction.from_dict(bonus_transaction_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


