This is an opsmx plugin repository that references plugins.

Adding the following to your orca.yml config will load and start the latest CustomStage plugin during app startup.
```
spinnaker:
  extensibility:
    plugins:
      Opsmx.CustomStagePlugin:
        enabled: true
        version: 1.0.1
        config:
          defaultVmDetails: abcd
          defaultgitAccount: ijkl
    repositories:
      example-repo:
        url: https://raw.githubusercontent.com/spinnaker-plugin-examples/examplePluginRepository/master/repositories.json
```
