# Azure Custom Policy
Azure Custom Policy to Scope VM which is migrated with Azure Migrate and has missing parameters "imagePublisher" "imageOffer" "imageSKU"

This repository contains Azure Policy definitions that can be used to scope virtual machines (VMs) that were not previously scoped by built-in policies. These policies can help ensure that your VMs are properly configured and secured.

## Usage

To use these policies, you'll need to import them into your Azure Policy environment. Here's how:

1. Clone this repository to your local machine.
2. Open the Azure Policy portal in your browser.
3. Click on "Definitions" in the left-hand menu.
4. Click on "Import definition" at the top of the page.
5. Select the JSON file for the policy you want to import (located in the "policies" folder of this repository).
6. Follow the prompts to complete the import process.

Once you've imported the policies, you can assign them to your VMs by creating an Azure Policy assignment. Here's how:

1. Click on "Assignments" in the left-hand menu of the Azure Policy portal.
2. Click on "Assign policy" at the top of the page.
3. Select the policy you want to assign from the list.
4. Follow the prompts to complete the assignment process.

## Policies

This repository contains the following policies:

- `policy1.json`: This policy scopes VMs to a specific subscription or resource group and remediates the scoped VM's with AMA extension
- `policy2.json`: This policy remediation tasks attaches DCR to VMs. (configure DCR prior creating policy2 since it's mandatory to provide DCR resource ID 

## Contributing

If you have suggestions for additional policies or improvements to existing policies, please feel free to submit a pull request or open an issue.

## License

This repository is licensed under the MIT License. See the `LICENSE` file for more information.

