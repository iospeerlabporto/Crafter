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
- Define Interactive Interface (questions to the user)
- Logic for Moving the Template into a new folder
- Logic for Replacing MACROS

(Optional)
- Logic for generating the `.swift` files with Stencil
- Add `swiftlint` support (add pod to Podfile and Run Script)
- Remove Main.storyboard
- Support for more Architectures (MVVM, MVP, CLEAN)
- Add Xcode Templates (?)

## Tech Notes
- Project is based on a created template in `/templates`
- Files within project are created using Stencil
- In case we want to use Cocoapods, run `pod install` in the end
- `.gitignore` is fetched from `https://www.gitignore.io/api/swift,xcode`
- `git init` with given remote