
# ua-jiraalign

The ConnectALL Jira Align Universal Adapter is developed as an extension to the universal adapter capability of ConnectALL. This adapter will allow the user to use Jira Align with ConnectALL. Current capabilities and limitations will be defined below.

Please refer to the [ConnectALL Tech Docs](https://techdocs.broadcom.com/us/en/ca-enterprise-software/valueops/connectall/3-5/adapters/universal-adapter.html) for more information.

If you are an existing SaaS customer, please contact Broadcom Support to enable the adapter in your environment. If you are using ConnectALL On-Premise, you may download and install this adapter in your environment. If you are not yet a customer, [please reach out to learn more](https://enterprise-software.broadcom.com/contact-us).

# Setup

## Supported Entities

This Universal Adapter currently supports the following entities:
* Portfolio Epics
* Features
* Primary Programs

*Note: This Universal Adapter is provided as-is. It is tested and validated using the entities and configurations as defined. Any additional customizations are not supported and should be made at your own discretion.*

## Connection Details

* **Connection Name:** *Name of Application*
* **Application Type:** Jira Align
* **URL:** *Base URL for application (ex: https://broadcom.com)*
* **User Name:** *Set if neccessary, recommend using the Service Account user name*
* **Password:** *Set if neccessary*
* **Application Category:** *Pick from dropdown list*
* **Time Zone:** Not required for Jira Align
* **Select Group:** *Set if neccessary*
* **Authentication Type:** ApiKey
* **API Key:** Authorization
* **API Value:** Bearer user:JiraAlignAPIKey

## Flow Filters

The filtering method for Jira Align is not known.

## Example Automation

Sync all Portoflio Epics with their child Features to Clarity, as a parent Custom Investment Type (CIT), with tasks as children on the CIT.

# Known Limitations

* You must be using v2 of the Jira Align API
* All fields are prefaced with issuetypedto-, you'll need to filter through the fields
* A filtering method for Flow Filters is not known
* Align appears to have fields that shown as non-required in the UI, but require a value to be set when using the API (your experience may vary)

# Supporting Documentation

Third Party API Documentation: [Link to API Documentation](https://help.jiraalign.com/hc/en-us/articles/360045371954-Getting-started-with-the-REST-API-2-0)
