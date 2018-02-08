# Bug example for Expo w/ React-native-firebase causing build errors.

## To install:

- Clone repo.
- run `npm install` in the root.
- run `pod install` in the `ios` directory.
- Open the generated `.xcworkspace`

This is a plain `create-react-native` app ejected to ExpoKit, then the firebase pods installed, then the `react-native-firebase` library installed, then linked using `react-native link react-native-firebase`.

Each step is included as commit in the repo, and screenshots of the errors are available in /Error-Screenshots under the short commit name it references.

- Possibly something to do with gRPC module/pod as that is where the conflicting type errors appear.
- Different number of errors for debug and release schemes.
- Happens if i try to build the `RNFirebase.xcodeproj` alone, too.
