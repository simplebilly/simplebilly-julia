# ReturnLogisticsSummary


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`byStatus`** | **`Any`** | Number of return orders per status. | [default to nothing]
**`byWarehouse`** | [**`Vector{ReturnWarehouseSummary}`**](ReturnWarehouseSummary.md) | Per-warehouse aggregation. | [default to nothing]
**`itemsRestocked`** | **`Int64`** | Sum of &#x60;restock: true&#x60; line-item quantities. | [default to nothing]
**`itemsScrapped`** | **`Int64`** | Sum of &#x60;restock: false&#x60; line-item quantities (scrapped/disposed). | [default to nothing]
**`totalItems`** | **`Int64`** | Sum of all line-item quantities across returns. | [default to nothing]
**`totalReturns`** | **`Int64`** | Total number of return orders (excluding soft-deleted). | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


