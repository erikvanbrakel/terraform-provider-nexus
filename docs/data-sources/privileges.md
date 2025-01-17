---
page_title: "Data Source nexus_privileges"
subcategory: "Other"
description: |-
  Use this data source to work with privileges.
---
# Data Source nexus_privileges
Use this data source to work with privileges.
## Example Usage
```terraform
data "nexus_privileges" "example" {
  domain     = "application"
  format     = "maven2"
  repository = "maven-public"
  type       = "repository-admin"
}
```
<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- **domain** (String) The domain of the privilege
- **format** (String) The format of the privilege
- **name** (String) The name of the privilege
- **repository** (String) The repository of the privilege
- **type** (String) The type of the privilege

### Read-Only

- **id** (String) Used to identify data source at nexus
- **privileges** (List of Object) List of privileges (see [below for nested schema](#nestedatt--privileges))

<a id="nestedatt--privileges"></a>
### Nested Schema for `privileges`

Read-Only:

- **actions** (Set of String)
- **content_selector** (String)
- **description** (String)
- **domain** (String)
- **format** (String)
- **name** (String)
- **pattern** (Boolean)
- **read_only** (Boolean)
- **repository** (String)
- **type** (String)

