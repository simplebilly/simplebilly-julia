# KonzernStatus


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`groessenbefreit`** | **`Bool`** |  | [default to nothing]
**`kapitalmarktorientiert`** | **`Bool`** |  | [default to nothing]
**`konzernabschlusspflicht`** | **`Bool`** |  | [default to nothing]
**`missing_group_figures`** | **`Bool`** | Keine group_figures-Zeile für das Jahr vorhanden → keine Größenbefreiung. | [default to nothing]
**`mutterunternehmen`** | **`Bool`** | Mutterunternehmen: mindestens eine beherrschte Beteiligung (§ 290 Abs. 1 HGB). | [default to nothing]
**`parent_name`** | **`String`** | Mutterunternehmen für die Zwischenholding-Befreiung (§ 291 HGB). | [optional] [default to nothing]
**`parent_situs`** | **`String`** |  | [optional] [default to nothing]
**`participations`** | [**`Vector{KonzernBeteiligung}`**](KonzernBeteiligung.md) |  | [default to nothing]
**`thresholds`** | [**`*KonzernThresholds`**](KonzernThresholds.md) |  | [default to nothing]
**`year`** | **`Int64`** |  | [default to nothing]
**`zwischenholding_befreit`** | **`Bool`** |  | [default to nothing]
**`zwischenholding_hinweis`** | **`String`** | Hinweis zu den § 291-Voraussetzungen (EU/EWR-Sitz, geprüfter Konzernabschluss). | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


