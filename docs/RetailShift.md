# RetailShift

Розничная смена

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Розничной смены | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование смены | [optional] 
**moment** | **str** | Дата смены | [optional] 
**retail_store** | [**RetailStore**](RetailStore.md) | Метаданные точки продаж | [optional] 
**payments** | [**List[RetailShiftPaymentsInner]**](RetailShiftPaymentsInner.md) | Связанные платежи | [optional] 
**acquire** | [**Agent**](Agent.md) | Метаданные Банка-эквайера по операциям по карте | [optional] 
**agent_account** | [**Account**](Account.md) | Метаданные счета контрагента | [optional] [readonly] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**bank_comission** | **float** | Сумма комиссии эквайера за проведение безналичных платежей по банковской карте | [optional] 
**bank_percent** | **float** | Комиссия банка-эквайера по операциям по карте (в процентах) | [optional] 
**cheque** | [**RetailShiftCheque**](RetailShiftCheque.md) | Информация о смене ККТ | [optional] 
**close_date** | **str** | Дата закрытия смены | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] [readonly] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Розничной смены | [optional] [readonly] 
**description** | **str** | Комментарий Розничной смены | [optional] 
**external_code** | **str** | Внешний код Розничной смены | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**group** | [**Group**](Group.md) | Отдел сотрудника | [optional] 
**operations** | [**List[RetailShiftOperation]**](RetailShiftOperation.md) | Связанные операции. Допустимые типы по &#x60;meta.type&#x60;: retaildemand, retailsalesreturn, retaildrawercashin, retaildrawercashout, prepayment, prepaymentreturn.  | [optional] [readonly] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета юрлица | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**payment_operations** | [**List[RetailShiftPaymentOperation]**](RetailShiftPaymentOperation.md) | Коллекция метаданных платежных операций | [optional] [readonly] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**proceeds_cash** | **float** | Выручка наличными | [optional] [readonly] 
**proceeds_no_cash** | **float** | Выручка безнал | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**qr_acquire** | [**Agent**](Agent.md) | Метаданные Банка-эквайера по операциям по QR-коду | [optional] 
**qr_bank_comission** | **float** | Сумма комиссии эквайера за проведение безналичных платежей по QR-коду | [optional] 
**qr_bank_percent** | **float** | Комиссия банка-эквайера по операция по QR-коду (в процентах) | [optional] 
**received_cash** | **float** | Получено наличными | [optional] [readonly] 
**received_no_cash** | **float** | Получено безнал | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**store** | [**Store**](Store.md) |  | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**updated** | **str** | Момент последнего обновления Розничной смены | [optional] [readonly] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] [readonly] 
**vat_included** | **bool** | Включен ли НДС в цену | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_shift import RetailShift

# TODO update the JSON string below
json = "{}"
# create an instance of RetailShift from a JSON string
retail_shift_instance = RetailShift.from_json(json)
# print the JSON string representation of the object
print(RetailShift.to_json())

# convert the object into a dict
retail_shift_dict = retail_shift_instance.to_dict()
# create an instance of RetailShift from a dict
retail_shift_from_dict = RetailShift.from_dict(retail_shift_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


