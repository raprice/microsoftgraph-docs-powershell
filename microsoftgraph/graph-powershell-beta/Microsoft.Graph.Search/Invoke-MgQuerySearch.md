---
external help file: Microsoft.Graph.Search-help.xml
Module Name: Microsoft.Graph.Search
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.search/invoke-mgquerysearch
schema: 2.0.0
---

# Invoke-MgQuerySearch

## SYNOPSIS
Run a specified search query.
Search results are provided in the response.

## SYNTAX

### QueryExpanded (Default)
```
Invoke-MgQuerySearch [-AdditionalProperties <Hashtable>] [-Requests <IMicrosoftGraphSearchRequest[]>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Query
```
Invoke-MgQuerySearch
 -BodyParameter <IPaths1Kd2XrlSearchMicrosoftGraphQueryPostRequestbodyContentApplicationJsonSchema> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Run a specified search query.
Search results are provided in the response.

## EXAMPLES

### Example 1: Using the Invoke-MgQuerySearch Cmdlet
```powershell
Import-Module Microsoft.Graph.Search
$params = @{
	Requests = @(
		@{
			EntityTypes = @(
				"externalItem"
			)
			ContentSources = @(
				"/external/connections/connectionfriendlyname"
			)
			Query = @{
				QueryString = "contoso product"
			}
			From = 0
			Size = 25
			Fields = @(
				"title"
				"description"
			)
		}
	)
}
Invoke-MgQuerySearch -BodyParameter $params
```

This example shows how to use the Invoke-MgQuerySearch Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: QueryExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
.
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPaths1Kd2XrlSearchMicrosoftGraphQueryPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Query
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Requests
.
To construct, please use Get-Help -Online and see NOTES section for REQUESTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphSearchRequest[]
Parameter Sets: QueryExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IPaths1Kd2XrlSearchMicrosoftGraphQueryPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphSearchResponse
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPaths1Kd2XrlSearchMicrosoftGraphQueryPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Requests <IMicrosoftGraphSearchRequest[]>]`: 
    - `[AggregationFilters <String[]>]`: Contains one or more filters to obtain search results aggregated and filtered to a specific value of a field. Optional.Build this filter based on a prior search that aggregates by the same field. From the response of the prior search, identify the searchBucket that filters results to the specific value of the field, use the string in its aggregationFilterToken property, and build an aggregation filter string in the format '{field}:/'{aggregationFilterToken}/''. If multiple values for the same field need to be provided, use the strings in its aggregationFilterToken property and build an aggregation filter string in the format '{field}:or(/'{aggregationFilterToken1}/',/'{aggregationFilterToken2}/')'. For example, searching and aggregating drive items by file type returns a searchBucket for the file type docx in the response. You can conveniently use the aggregationFilterToken returned for this searchBucket in a subsequent search query and filter matches down to drive items of the docx file type. Example 1 and example 2 show the actual requests and responses.
    - `[Aggregations <IMicrosoftGraphAggregationOption[]>]`: Specifies aggregations (also known as refiners) to be returned alongside search results. Optional.
      - `[BucketDefinition <IMicrosoftGraphBucketAggregationDefinition>]`: bucketAggregationDefinition
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[IsDescending <Boolean?>]`: True to specify the sort order as descending. The default is false, with the sort order as ascending. Optional.
        - `[MinimumCount <Int32?>]`: The minimum number of items that should be present in the aggregation to be returned in a bucket. Optional.
        - `[PrefixFilter <String>]`: A filter to define a matching criteria. The key should start with the specified prefix to be returned in the response. Optional.
        - `[Ranges <IMicrosoftGraphBucketAggregationRange[]>]`: Specifies the manual ranges to compute the aggregations. This is only valid for non-string refiners of date or numeric type. Optional.
          - `[From <String>]`: Defines the lower bound from which to compute the aggregation. This can be a numeric value or a string representation of a date using the YYYY-MM-DDTHH:mm:ss.sssZ format. Required.
          - `[To <String>]`: Defines the upper bound up to which to compute the aggregation. This can be a numeric value or a string representation of a date using the YYYY-MM-DDTHH:mm:ss.sssZ format. Required.
        - `[SortBy <String>]`: bucketAggregationSortProperty
      - `[Field <String>]`: Computes aggregation on the field while the field exists in current entity type. Required.
      - `[Size <Int32?>]`: The number of searchBucket resources to be returned. This is not required when the range is provided manually in the search request. Optional.
    - `[CollapseProperties <IMicrosoftGraphCollapseProperty[]>]`: Contains the ordered collection of fields and limit to collapse results. Optional.
      - `[Fields <String[]>]`: Defines the collapse group to trim results. The properties in this collection must be sortable/refinable properties. Required.
      - `[Limit <Int32?>]`: Defines a maximum limit count for this field. This numeric value must be a positive integer. Required.
    - `[ContentSources <String[]>]`: Contains the connection to be targeted. Respects the following format : /external/connections/connectionid where connectionid is the ConnectionId defined in the Connectors Administration.  Note: contentSource is only applicable when entityType=externalItem. Optional.
    - `[EnableTopResults <Boolean?>]`: This triggers hybrid sort for messages: the first 3 messages are the most relevant. This property is only applicable to entityType=message. Optional.
    - `[EntityTypes <String[]>]`: One or more types of resources expected in the response. Possible values are: list, site, listItem, message, event, drive, driveItem, person, externalItem, acronym, bookmark, chatMessage. For details about combinations of two or more entity types that are supported in the same search request, see known limitations. Required.
    - `[Fields <String[]>]`: Contains the fields to be returned for each resource object specified in entityTypes, allowing customization of the fields returned by default otherwise, including additional fields such as custom managed properties from SharePoint and OneDrive, or custom fields in externalItem from content that Microsoft Graph connectors bring in. The fields property can be using the semantic labels applied to properties. For example, if a property is label as title, you can retrieve it using the following syntax : label_title.Optional.
    - `[From <Int32?>]`: Specifies the offset for the search results. Offset 0 returns the very first result. Optional.
    - `[Query <IMicrosoftGraphSearchQuery1>]`: searchQuery
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[QueryString <String>]`: The search query containing the search terms. Required.
      - `[QueryString1 <IMicrosoftGraphSearchQueryString2>]`: searchQueryString
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Query <String>]`: Contains the actual search terms of the request.
      - `[QueryTemplate <String>]`: Provides a way to decorate the query string. Supports both KQL and query variables. Optional.
    - `[QueryAlterationOptions <IMicrosoftGraphSearchAlterationOptions>]`: searchAlterationOptions
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[EnableModification <Boolean?>]`: Indicates whether spelling modifications are enabled. If enabled, the user will get the search results for the corrected query in case of no results for the original query with typos. The response will also include the spelling modification information in the queryAlterationResponse property. Optional.
      - `[EnableSuggestion <Boolean?>]`: Indicates whether spelling suggestions are enabled. If enabled, the user will get the search results for the original search query and suggestions for spelling correction in the queryAlterationResponse property of the response for the typos in the query. Optional.
    - `[Region <String>]`: Required for searches that use application permissions. Represents the geographic location for the search. For details, see Get the region value.
    - `[ResultTemplateOptions <IMicrosoftGraphResultTemplateOption>]`: resultTemplateOption
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[EnableResultTemplate <Boolean?>]`: Indicates whether search display layouts are enabled. If enabled, the user will get the result template to render the search results content in the resultTemplates property of the response. The result template is based on Adaptive Cards. Optional.
    - `[SharePointOneDriveOptions <IMicrosoftGraphSharePointOneDriveOptions>]`: sharePointOneDriveOptions
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IncludeContent <String>]`: searchContent
    - `[Size <Int32?>]`: The size of the page to be retrieved. Optional.
    - `[SortProperties <IMicrosoftGraphSortProperty[]>]`: Contains the ordered collection of fields and direction to sort results. There can be at most 5 sort properties in the collection. Optional.
      - `[IsDescending <Boolean?>]`: True if the sort order is descending. Default is false, with the sort order as ascending. Optional.
      - `[Name <String>]`: The name of the property to sort on. Required.
    - `[StoredFields <String[]>]`: 
    - `[TrimDuplicates <Boolean?>]`: Indicates whether to trim away the duplicate SharePoint files from search results. Default value is false. Optional.

REQUESTS <IMicrosoftGraphSearchRequest\[]>: .
  - `[AggregationFilters <String[]>]`: Contains one or more filters to obtain search results aggregated and filtered to a specific value of a field. Optional.Build this filter based on a prior search that aggregates by the same field. From the response of the prior search, identify the searchBucket that filters results to the specific value of the field, use the string in its aggregationFilterToken property, and build an aggregation filter string in the format '{field}:/'{aggregationFilterToken}/''. If multiple values for the same field need to be provided, use the strings in its aggregationFilterToken property and build an aggregation filter string in the format '{field}:or(/'{aggregationFilterToken1}/',/'{aggregationFilterToken2}/')'. For example, searching and aggregating drive items by file type returns a searchBucket for the file type docx in the response. You can conveniently use the aggregationFilterToken returned for this searchBucket in a subsequent search query and filter matches down to drive items of the docx file type. Example 1 and example 2 show the actual requests and responses.
  - `[Aggregations <IMicrosoftGraphAggregationOption[]>]`: Specifies aggregations (also known as refiners) to be returned alongside search results. Optional.
    - `[BucketDefinition <IMicrosoftGraphBucketAggregationDefinition>]`: bucketAggregationDefinition
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsDescending <Boolean?>]`: True to specify the sort order as descending. The default is false, with the sort order as ascending. Optional.
      - `[MinimumCount <Int32?>]`: The minimum number of items that should be present in the aggregation to be returned in a bucket. Optional.
      - `[PrefixFilter <String>]`: A filter to define a matching criteria. The key should start with the specified prefix to be returned in the response. Optional.
      - `[Ranges <IMicrosoftGraphBucketAggregationRange[]>]`: Specifies the manual ranges to compute the aggregations. This is only valid for non-string refiners of date or numeric type. Optional.
        - `[From <String>]`: Defines the lower bound from which to compute the aggregation. This can be a numeric value or a string representation of a date using the YYYY-MM-DDTHH:mm:ss.sssZ format. Required.
        - `[To <String>]`: Defines the upper bound up to which to compute the aggregation. This can be a numeric value or a string representation of a date using the YYYY-MM-DDTHH:mm:ss.sssZ format. Required.
      - `[SortBy <String>]`: bucketAggregationSortProperty
    - `[Field <String>]`: Computes aggregation on the field while the field exists in current entity type. Required.
    - `[Size <Int32?>]`: The number of searchBucket resources to be returned. This is not required when the range is provided manually in the search request. Optional.
  - `[CollapseProperties <IMicrosoftGraphCollapseProperty[]>]`: Contains the ordered collection of fields and limit to collapse results. Optional.
    - `[Fields <String[]>]`: Defines the collapse group to trim results. The properties in this collection must be sortable/refinable properties. Required.
    - `[Limit <Int32?>]`: Defines a maximum limit count for this field. This numeric value must be a positive integer. Required.
  - `[ContentSources <String[]>]`: Contains the connection to be targeted. Respects the following format : /external/connections/connectionid where connectionid is the ConnectionId defined in the Connectors Administration.  Note: contentSource is only applicable when entityType=externalItem. Optional.
  - `[EnableTopResults <Boolean?>]`: This triggers hybrid sort for messages: the first 3 messages are the most relevant. This property is only applicable to entityType=message. Optional.
  - `[EntityTypes <String[]>]`: One or more types of resources expected in the response. Possible values are: list, site, listItem, message, event, drive, driveItem, person, externalItem, acronym, bookmark, chatMessage. For details about combinations of two or more entity types that are supported in the same search request, see known limitations. Required.
  - `[Fields <String[]>]`: Contains the fields to be returned for each resource object specified in entityTypes, allowing customization of the fields returned by default otherwise, including additional fields such as custom managed properties from SharePoint and OneDrive, or custom fields in externalItem from content that Microsoft Graph connectors bring in. The fields property can be using the semantic labels applied to properties. For example, if a property is label as title, you can retrieve it using the following syntax : label_title.Optional.
  - `[From <Int32?>]`: Specifies the offset for the search results. Offset 0 returns the very first result. Optional.
  - `[Query <IMicrosoftGraphSearchQuery1>]`: searchQuery
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[QueryString <String>]`: The search query containing the search terms. Required.
    - `[QueryString1 <IMicrosoftGraphSearchQueryString2>]`: searchQueryString
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Query <String>]`: Contains the actual search terms of the request.
    - `[QueryTemplate <String>]`: Provides a way to decorate the query string. Supports both KQL and query variables. Optional.
  - `[QueryAlterationOptions <IMicrosoftGraphSearchAlterationOptions>]`: searchAlterationOptions
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[EnableModification <Boolean?>]`: Indicates whether spelling modifications are enabled. If enabled, the user will get the search results for the corrected query in case of no results for the original query with typos. The response will also include the spelling modification information in the queryAlterationResponse property. Optional.
    - `[EnableSuggestion <Boolean?>]`: Indicates whether spelling suggestions are enabled. If enabled, the user will get the search results for the original search query and suggestions for spelling correction in the queryAlterationResponse property of the response for the typos in the query. Optional.
  - `[Region <String>]`: Required for searches that use application permissions. Represents the geographic location for the search. For details, see Get the region value.
  - `[ResultTemplateOptions <IMicrosoftGraphResultTemplateOption>]`: resultTemplateOption
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[EnableResultTemplate <Boolean?>]`: Indicates whether search display layouts are enabled. If enabled, the user will get the result template to render the search results content in the resultTemplates property of the response. The result template is based on Adaptive Cards. Optional.
  - `[SharePointOneDriveOptions <IMicrosoftGraphSharePointOneDriveOptions>]`: sharePointOneDriveOptions
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IncludeContent <String>]`: searchContent
  - `[Size <Int32?>]`: The size of the page to be retrieved. Optional.
  - `[SortProperties <IMicrosoftGraphSortProperty[]>]`: Contains the ordered collection of fields and direction to sort results. There can be at most 5 sort properties in the collection. Optional.
    - `[IsDescending <Boolean?>]`: True if the sort order is descending. Default is false, with the sort order as ascending. Optional.
    - `[Name <String>]`: The name of the property to sort on. Required.
  - `[StoredFields <String[]>]`: 
  - `[TrimDuplicates <Boolean?>]`: Indicates whether to trim away the duplicate SharePoint files from search results. Default value is false. Optional.

## RELATED LINKS

## RELATED LINKS
