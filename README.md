# testIssueTracking
"trackedInIssues": {             "totalCount": 0, error ?

the followig query seems buggy 


```
gh api graphql -f query='
{
  search(query: "repo:heindel/testIssueTracking in:title The issue with lots of tracking", type: ISSUE, first: 1) {
    issueCount
    nodes {
      ... on Issue {
        number
        title
        body
        url
        trackedInIssues(first: 2){
            totalCount
            nodes {
                url
            }
        }
        labels(first: 2) {
            totalCount
            nodes {
                color
            }
        }
      }
    }
  }
}'
```
