# publish-stack-action

[![Action test](https://github.com/stack-spot/workflow-github-action-publish-stack/actions/workflows/action-test.yml/badge.svg)](https://github.com/stack-spot/workflow-github-action-publish-stack/actions/workflows/action-test.yml)

GitHub action to publish stack

## 📚 Usage

### Requirements

To learn more about generating account keys(`CLIENT_ID`, `CLIENT_KEY`, `REALM`), please refer to the documentation:
https://docs.stackspot.com/en/home/set-up/customization/access-token

### Use Case

```yaml
    steps:
      - uses: stack-spot/workflow-github-action-publish-stack@v1
        with:
          client_id: ${{ secrets.CLIENT_ID }}
          client_key: ${{ secrets.CLIENT_KEY }}
          realm: ${{ secrets.REALM }}
          studio: studio_name
          stack_path: stack_path #optional
```

## License

[Apache License 2.0](https://github.com/stack-spot/publish-plugin-action/blob/main/LICENSE)
