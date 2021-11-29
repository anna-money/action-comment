# Add or update comment GitHub Action

This action allows you to create or update comment in your PR.

## Inputs

1. `text` (string, required) - text to place in comment
2. `search_key` (string, required) - text to search existing comment
3. `timezone` (string, default: `'UTC'`) - timezone for comment update timestamp

## Example

Write in your workflow:

```yml
upsert-comment:
  runs-on: ubuntu-latest
  steps:
    - uses: anna-money/action-comment@master
      with:
        timezone: 'Europe/Moscow'
        search_key: 'Coverage'
        text: |
          #### Coverage
          ```
          <coverage report>
          ```
```

Result:
![example](images/example.png)