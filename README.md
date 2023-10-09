# repo-rules-security-checks-demo
demo of using repo rules to enforce seurity checks

## How This Works

To ensure security scans are ran, you can use a combination of: 
1. Reusable Workflows
2. Repository Rulesets, and 
3. Required Status Checks, with the name of the job in the calling workflow and the name of the job in the reusable workflow separated by a space, forward slash, space
   - For example:  `security-checks / security-checks`

- To ensure certain workflows aren’t updated, use the Codeowners file
Example: compliance-*.yml workflows are owned by the security team


## Notes

- Use this script to push workflow to selected repositories https://github.com/joshjohanning/github-misc-scripts/blob/main/gh-cli/add-workflow-file-to-repositories.sh
