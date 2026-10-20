---
'@adcp/sdk': patch
---

`resolvePropertyList` and `resolveCollectionList` now read the list from MCP `structuredContent` or a JSON text block, so resolving over the default MCP transport no longer fails with `property_list_invalid_response`. An MCP error result keeps its `adcp_error` on `error.cause`.
