# Code Scanning Alerts Workflow

This sample GitHub workflow demonstrates how the GitHub CLI can be used to retrieve
and analyze results, displaying them as part of the build output using Markdown. 
Optionally, the workflow can use Bash scripting and the CLI to dynamically reset the
status for dismissed alerts to `open`.

## Additional features

The code also demonstrates:

- How to dynamically create environment variables for a job (by appending data to $GITHUB_ENV)
- Illustrates differences in behavior for `${{ env.variable }}` expressions compared to 
using Bash `$VARIABLE`.
- Creating Markdown-based build outputs (using $GITHUB_STEP_SUMMARY)
- Using `jq` to process data
- Using `@base64` to make it easier to process rows of data in Bash
