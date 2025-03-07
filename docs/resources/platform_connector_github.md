---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "harness_platform_connector_github Resource - terraform-provider-harness"
subcategory: "NextGen"
description: |-
  Resource for creating a Github connector.
---

# harness_platform_connector_github (Resource)

Resource for creating a Github connector.



<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `connection_type` (String) Whether the connection we're making is to a github repository or a github account. Valid values are Account, Repo.
- `credentials` (Block List, Min: 1, Max: 1) Credentials to use for the connection. (see [below for nested schema](#nestedblock--credentials))
- `identifier` (String) Unique identifier of the resource.
- `name` (String) Name of the resource.
- `url` (String) Url of the Githubhub repository or account.

### Optional

- `api_authentication` (Block List, Max: 1) Configuration for using the github api. API Access is required for using “Git Experience”, for creation of Git based triggers, Webhooks management and updating Git statuses. (see [below for nested schema](#nestedblock--api_authentication))
- `delegate_selectors` (Set of String) Connect using only the delegates which have these tags.
- `description` (String) Description of the resource.
- `org_id` (String) Unique identifier of the organization.
- `project_id` (String) Unique identifier of the project.
- `tags` (Set of String) Tags to associate with the resource. Tags should be in the form `name:value`.
- `validation_repo` (String) Repository to test the connection with. This is only used when `connection_type` is `Account`.

### Read-Only

- `id` (String) The ID of this resource.

<a id="nestedblock--credentials"></a>
### Nested Schema for `credentials`

Optional:

- `http` (Block List, Max: 1) Authenticate using Username and password over http(s) for the connection. (see [below for nested schema](#nestedblock--credentials--http))
- `ssh` (Block List, Max: 1) Authenticate using SSH for the connection. (see [below for nested schema](#nestedblock--credentials--ssh))

<a id="nestedblock--credentials--http"></a>
### Nested Schema for `credentials.http`

Required:

- `token_ref` (String) Reference to a secret containing the personal access to use for authentication.

Optional:

- `username` (String) Username to use for authentication.
- `username_ref` (String) Reference to a secret containing the username to use for authentication.


<a id="nestedblock--credentials--ssh"></a>
### Nested Schema for `credentials.ssh`

Required:

- `ssh_key_ref` (String) Reference to the Harness secret containing the ssh key.



<a id="nestedblock--api_authentication"></a>
### Nested Schema for `api_authentication`

Optional:

- `github_app` (Block List, Max: 1) Configuration for using the github app for interacting with the github api. (see [below for nested schema](#nestedblock--api_authentication--github_app))
- `token_ref` (String) Personal access token for interacting with the github api.

<a id="nestedblock--api_authentication--github_app"></a>
### Nested Schema for `api_authentication.github_app`

Required:

- `application_id` (String) Enter the GitHub App ID from the GitHub App General tab.
- `installation_id` (String) Enter the Installation ID located in the URL of the installed GitHub App.
- `private_key_ref` (String) Reference to the secret containing the private key.


