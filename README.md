# beastmatch - sample game for iOS

```
trigger:
- master

pool:
  vmImage: 'macos-latest'

steps:
- task: Xcode@5
  inputs:
    actions: 'test'
    scheme: 'BeastMatchTests'
    sdk: 'iphonesimulator'
    configuration: 'Debug'
    destinationPlatformOption: 'iOS'
    publishJUnitResults: true
    
```
