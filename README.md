# SourceryTemplates
sourcery templates


`git clone git@github.com:danramteke/SourceryTemplates.git ~/.SourceryTemplates`

And then in your sourcery config file, you can refer to this directory

file: .sourcery.yml
```
sources:
  - ./Tests/
templates:
  - ~/.SourceryTemplates/LinuxMain.stencil
output: ./Tests/LinuxMain.swift
args:
  testimports: "@testable import UnderwayHeartbeatTests"
```

then you can run `mint run Sourcery` in your project's root directory to update your `LinuxMain.swift`


Sourcery: https://github.com/krzysztofzablocki/Sourcery#configuration-file

Mint: https://github.com/yonaskolb/Mint
