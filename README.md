#  Crafter
## iOS and macOS Project Bootstrapper

### Generate a new Folder with 
- starter Podfile
- starter Gemfile
- .gitignore
- Fastfile
- License
- README

### Xcode Proj
- MVC
- Supporting Files
- Custom build configurations (Debug, AdHoc and Release) with custom Bundle Identifiers

### Project Structure
```
PROJECTNAME
|- 🗂 PROJECTNAME
  |- 🗂 AppDelegate
    |- AppDelegate.swift (generated)
  |- 🗂 Controllers
    |- ViewController.swift (generated)
  |- 🗂 Models
  |- 🗂 Resources
    |- 🗂 Assets.xcassets
  |- 🗂 Supporting Files
  |- 🗂 Views
|- PROJECTNAME.xcodeproj
|- .gitignore
|- README.md
|- LICENSE.md
|- Podfile (optional)
|- 🗂 Fastlane (optional)
  |- Fastfile
```

TODO
- Add `swiftlint` support (add pod to Podfile and Run Script)
- Remove Main.storyboard



## Tech Notes
- Project is based on a created template in `/templates`
- Files within project are created using Stencil
- In case we want to use Cocoapods, run `pod install` in the end
- `.gitignore` is fetched from `https://www.gitignore.io/api/swift,xcode`
- `git init` with given remote