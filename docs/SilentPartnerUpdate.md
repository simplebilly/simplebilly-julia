# SilentPartnerUpdate


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`contractDate`** | **`Date`** | Datum des Vertragsabschlusses. | [optional] [default to nothing]
**`einlage`** | **`String`** | Einlage (§ 230 HGB). | [optional] [default to nothing]
**`gewinnquotePct`** | **`String`** | Gewinnbeteiligungsquote in Prozent (§ 231 HGB). | [optional] [default to nothing]
**`gewinnvortrag`** | **`String`** | Nicht erhobene Gewinne (§ 232 Abs. 3 HGB). | [optional] [default to nothing]
**`instrumentType`** | [**`*InstrumentType`**](InstrumentType.md) | Instrument: \&quot;typisch\&quot; | \&quot;atypisch\&quot; | \&quot;partiarisches_darlehen\&quot; | \&quot;genussrecht\&quot;. | [optional] [default to nothing]
**`kestPflichtig`** | **`Bool`** | 25 % Kapitalertragsteuer einbehalten (§ 43 Abs. 1 Nr. 3 EStG; typisch + partiarisches Darlehen). | [optional] [default to nothing]
**`name`** | **`String`** | Name des stillen Gesellschafters. | [optional] [default to nothing]
**`notes`** | **`String`** | Freitext-Notizen. | [optional] [default to nothing]
**`verlustVerrechnungskonto`** | **`String`** | Kumulierte Verluste gegen die Einlage (§ 232 Abs. 2 HGB, ≤ Einlage). | [optional] [default to nothing]
**`verlustbeteiligung`** | **`Bool`** | Verlustbeteiligung (§ 231 Abs. 2 HGB; kann ausgeschlossen werden). | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


