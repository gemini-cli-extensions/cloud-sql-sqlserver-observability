# Gemini CLI Extension - Cloud SQL for SQL Server Observability

This Gemini CLI extension provides a set of tools to interact with [Cloud SQL for SQL Server](https://cloud.google.com/sql/docs/sqlserver)  monitoring metrics. It allows you to fetch a wide range of database metrics, enabling comprehensive monitoring of database performance and health directly from the [Gemini CLI](https://google-gemini.github.io/gemini-cli/), using natural language prompts.

Learn more about [Gemini CLI Extensions](https://github.com/google-gemini/gemini-cli/blob/main/docs/extension.md)

## Why Use the Cloud SQL for SQL Server Observability Extension?

* **Natural Language Management:** Stop wrestling with complex monitoring queries. Explore monitoring data by describing what you want in plain English.
* **Seamless Workflow:** As a Google-developed extension, it integrates seamlessly into the Gemini CLI environment. No need to constantly switch contexts for common tasks.

## Prerequisites

Before you begin, ensure you have the following:

*   [Gemini CLI](https://github.com/google-gemini/gemini-cli) installed.
*   A Google Cloud project with the **Cloud Monitoring API** enabled.
*   IAM Permissions
    * Monitoring Viewer (`roles/monitoring.viewer`)

## Installation

To install the extension, use the command:

```bash
gemini extensions install github.com/gemini-cli-extensions/cloud-sql-sqlserver-observability
```

## Configuration

No configuration is required.

## Usage Examples

Interact with Cloud Monitoring metrics using natural language right from your IDE:

* "What is the memory usage for my SQL Server database?"
* "What is the overall system performance for my instance?"
* "What queries have been run for this instance over the last 3 hours?"
* "Provide the execution time for the query X"

## Supported Tools

* `get_system_metrics`: Fetches system level cloud monitoring data (timeseries metrics) for a SQL Server instance using a PromQL query.
* `get_query_metrics`: Fetches query level cloud monitoring data (timeseries metrics) for queries running in SQL Server instance using a PromQL query.

## Additional Extensions

Find additional extensions to support your entire software development lifecycle at [github.com/gemini-cli-extensions](https://github.com/gemini-cli-extensions).

## Troubleshooting

* "cannot execute binary file": Ensure the correct binary for your OS/Architecture has been downloaded. See [Installing the server](https://googleapis.github.io/genai-toolbox/getting-started/introduction/#installing-the-server) for more information.

