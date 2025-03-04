---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "aquasec_permissions_sets Data Source - terraform-provider-aquasec"
subcategory: ""
description: |-
  The data source aquasec_permissions_sets provides a method to query all permissions within the Aqua CSPMThe fields returned from this query are detailed in the Schema section below.
---

# Data Source `aquasec_permissions_sets`

The data source `aquasec_permissions_sets` provides a method to query all permissions within the Aqua CSPMThe fields returned from this query are detailed in the Schema section below.

## Example Usage

```terraform
data "aquasec_permissions_sets" "testpermissionsset" {}

output "permissions_sets" {
  value = data.aquasec_permissions_sets.testpermissionsset
}

output "permissions_sets_names" {
  value = data.aquasec_permissions_sets.testpermissionsset[*].permissions_sets[*].name
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- **id** (String) The ID of this resource.

### Read-only

- **permissions_sets** (List of Object) (see [below for nested schema](#nestedatt--permissions_sets))

<a id="nestedatt--permissions_sets"></a>
### Nested Schema for `permissions_sets`

Read-only:

- **actions** (List of String)
- **author** (String)
- **description** (String)
- **is_super** (Boolean)
- **name** (String)
- **ui_access** (Boolean)
- **updated_at** (String)


