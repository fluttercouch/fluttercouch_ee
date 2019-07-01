# Fluttercouch
With Fluttercouch is possible to use Couchbase Mobile Native SDK in Flutter Projects.

The plugin takes advantage of Flutter ability to write platform specific code to instantiate and manage a Couchbase Lite database. The Fluttercouch library is a wrapper to native SDK, which is handled from Dart through “mockup” objects. Those objects are responsible for creating local database, making CRUD operation and interact with a Couchbase database through platform channels.

None of the Dart object holds the actual state (which is hold in the native code). They are an interface to operate the native SDK in an easy and workable manner, helping developers to not deal with native layer directly.

## Installation

In order to use Fluttercouch, add this code to pubspec.yaml in your project directory. (Thanks to DhudumVishal)
```  fluttercouch: 
    git: 
      url: git://github.com/oltrenuovefrontiere/fluttercouch.git
```
The standard installation mode through pub.dartlang.org will be available in further releases.

NOTES:
- The current version uses the Couchbase Lite SDK 2.1 for Android and iOs.
- Due to Couchbase Lite SDK restrictions, the minSdkVersion for Android is 19 (Android KitKat 4.4) and minimum platform for iOs is 9.0

## Code Reference

Here will be listed code reference to Enteprise only features. For any other information on how to use this library, please refer to the base [Fluttercouch Library](https://github.com/fluttercouch/fluttercouch/blob/master/README.md).

### Encryption