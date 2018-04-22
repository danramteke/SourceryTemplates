# SourceryTemplates

## Usage

1. `git clone git@github.com:danramteke/SourceryTemplates.git ~/.SourceryTemplates`

2. In your Sourcery config file in your project's root directory, you can refer to this template directory. Here is an example `.sourcery.yml` file:

```
sources:
  - ./Tests/
templates:
  - ~/.SourceryTemplates/LinuxMain.stencil
output: ./Tests/LinuxMain.swift
args:
  testimports: "@testable import UnderwayHeartbeatTests"
```

3. Use Mint to run Sourcery. `mint run Sourcery` in your project's root directory to update your `LinuxMain.swift`


## Referenced Projects

- Sourcery: https://github.com/krzysztofzablocki/Sourcery#configuration-file
- Mint: https://github.com/yonaskolb/Mint
