# Vansah for Jira Action

... a GitHub action to import test results into Vansah for Jira

# Setup
 Do not specify username and password in cleartext, instead prefer to read them from GitHub action secrets.
## Configure the workflow
    runs-on: ubuntu-latest
    steps:
      -name: Sending results file to Vansah for Jira
      - uses: kawnkush/VansahIntegration@v10
        with:
            vansahToken: ${{secrets.vansahToken}}
            testPaths: "dummy.txt"
            log_identifier: 11050
            comment: "311331"
## Action outputs
 ${{steps.{VANSAH_STEP_ID}.outputs.count}}
 
 ${{steps.vansah.outputs.count}}

# Vansah
"Vansah" website 

# Developed By
Shubham Mourya

Ali Charara

shubham.mourya@testpoint.com.au

alicha@testpoint.com.au
