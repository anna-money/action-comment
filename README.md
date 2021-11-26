# Add or update comment GitHub Action
## Example
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
![example](images/example.png)