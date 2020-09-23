# speee/terraform-apply-action

The `speee/terraform-apply-action` action is a CI action that runs `terraform apply` when some commits are pushed to target branch.

## Usage

```yaml
- uses: speee/terraform-apply-action@v1
  with:
      terraform_version: 0.13.3
```

## Inputs

The action supports the following inputs:

- `working-directory` - (optional) Relative path from repository root to your terraform root module (default `.`).

- `aws-access-key-id` - (optional) Used when performing `terraform plan` to your AWS environment.

- `aws-secret-access-key` - (optional)

- `terraform-version` - (optional) The version of Terraform CLI to install. Defaults to `latest`.

- `github-token` - Used when writing comments on your pull request.
