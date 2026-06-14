# .github — Repository Automation & Template Configuration

This repository contains organization-wide configuration and GitHub Actions starter workflows for the **DeltaTest** (`deltatest-dev`) organization.

---

## 🚀 Starter Workflows

### DeltaTest (Smart Affected Test Runner)
Accelerate your CI/CD pipeline by executing only the `pytest` test suites affected by your git changes, instead of running the whole suite every time.

* **Workflow Template**: [.github/workflow-templates/deltatest.yml](.github/workflow-templates/deltatest.yml)
* **Metadata**: [.github/workflow-templates/deltatest.properties.json](.github/workflow-templates/deltatest.properties.json)

### How to Use in Organization Repositories
When you create a new GitHub Actions workflow in any repository under the `deltatest-dev` organization, this template will be suggested automatically under **"Workflows created by deltatest-dev"**.

1. Navigate to the **Actions** tab of your repository.
2. Click **New workflow**.
3. Select **Configure** under the **DeltaTest (Smart Affected Test Runner)** template.
4. Commit the generated `.github/workflows/deltatest.yml` file to your default branch.
5. Configure credentials in your repository under **Settings** → **Secrets and variables** → **Actions**:
   - `DELTA_API_KEY`: Your DeltaTest organization/user API key.
   - `DELTA_REPO_ID`: The unique repository ID from your DeltaTest dashboard.

---

## 📁 Directory Structure
