---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "harness_platform_connector_git Data Source - terraform-provider-harness"
subcategory: "NextGen"
description: |-
  Datasource for looking up a Git connector.
---

# harness_platform_connector_git (Data Source)

Datasource for looking up a Git connector.



<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `identifier` (String) Unique identifier of the resource.
- `name` (String) Name of the resource.
- `org_id` (String) Unique identifier of the organization.
- `project_id` (String) Unique identifier of the project.

### Read-Only

- `connection_type` (String) Whether the connection we're making is to a git repository or a git account. Valid values are Account, Repo.
- `credentials` (List of Object) Credentials to use for the connection. (see [below for nested schema](#nestedatt--credentials))
- `delegate_selectors` (Set of String) Connect using only the delegates which have these tags.
- `description` (String) Description of the resource.
- `id` (String) The ID of this resource.
- `tags` (Set of String) Tags to associate with the resource. Tags should be in the form `name:value`.
- `url` (String) Url of the git repository or account.
- `validation_repo` (String) Repository to test the connection with. This is only used when `connection_type` is `Account`.

<a id="nestedatt--credentials"></a>
### Nested Schema for `credentials`

Read-Only:

- `http` (List of Object) (see [below for nested schema](#nestedobjatt--credentials--http))
- `ssh` (List of Object) (see [below for nested schema](#nestedobjatt--credentials--ssh))

<a id="nestedobjatt--credentials--http"></a>
### Nested Schema for `credentials.http`

Read-Only:

- `password_ref` (String)
- `username` (String)
- `username_ref` (String)


<a id="nestedobjatt--credentials--ssh"></a>
### Nested Schema for `credentials.ssh`

Read-Only:

- `ssh_key_ref` (String)


