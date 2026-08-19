# FinanceInOperationCommissionReportIn

Полученный отчет комиссионера + linkedSum

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Полученного отчета комиссионера | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица | [optional] 
**agent_account** | [**Account**](Account.md) | Метаданные счета контрагента | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**code** | **str** | Код Полученного отчета комиссионера | [optional] 
**commission_overhead** | [**CommissionReportInCommissionOverhead**](CommissionReportInCommissionOverhead.md) |  | [optional] 
**commission_period_end** | **str** | Конец периода | [optional] 
**commission_period_start** | **str** | Начало периода | [optional] 
**commitent_sum** | **float** | Сумма коммитента в установленной валюте | [optional] [readonly] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Полученного отчета комиссионера | [optional] [readonly] 
**description** | **str** | Комментарий Полученного отчета комиссионера | [optional] 
**external_code** | **str** | Внешний код Полученного отчета комиссионера | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива файлов | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**name** | **str** | Наименование Полученного отчета комиссионера | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета юрлица | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**payed_sum** | **float** | Оплаченная сумма | [optional] [readonly] 
**positions** | [**CommissionReportInPositionList**](CommissionReportInPositionList.md) |  | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**return_to_commissioner_positions** | [**CommissionReportInReturnedPositionList**](.md) |  | [optional] 
**reward_percent** | **int** | Процент вознаграждения | [optional] 
**reward_type** | **str** | Тип Вознаграждения. Известные значения описаны в RewardType | [optional] 
**sales_channel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Полученного отчета комиссионера | [optional] 
**sum** | **float** | Сумма Полученного отчета комиссионера в копейках | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**updated** | **str** | Момент последнего обновления Полученного отчета комиссионера | [optional] [readonly] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] 
**vat_included** | **bool** | Включен ли НДС в цену | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] 
**payments** | [**List[RetailShiftPaymentsInner]**](RetailShiftPaymentsInner.md) | Массив ссылок на связанные платежи | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.finance_in_operation_commission_report_in import FinanceInOperationCommissionReportIn

# TODO update the JSON string below
json = "{}"
# create an instance of FinanceInOperationCommissionReportIn from a JSON string
finance_in_operation_commission_report_in_instance = FinanceInOperationCommissionReportIn.from_json(json)
# print the JSON string representation of the object
print(FinanceInOperationCommissionReportIn.to_json())

# convert the object into a dict
finance_in_operation_commission_report_in_dict = finance_in_operation_commission_report_in_instance.to_dict()
# create an instance of FinanceInOperationCommissionReportIn from a dict
finance_in_operation_commission_report_in_from_dict = FinanceInOperationCommissionReportIn.from_dict(finance_in_operation_commission_report_in_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


