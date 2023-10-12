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
$a^2$

**The Cauchy-Schwarz Inequality**
$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$

**The Cauchy-Schwarz Inequality**

```math
\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)
```
