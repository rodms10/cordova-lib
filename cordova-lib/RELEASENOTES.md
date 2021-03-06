<!--
#
# Licensed to the Apache Software Foundation (ASF) under one
# or more contributor license agreements.  See the NOTICE file
# distributed with this work for additional information
# regarding copyright ownership.  The ASF licenses this file
# to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance
# with the License.  You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing,
# software distributed under the License is distributed on an
# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
#  KIND, either express or implied.  See the License for the
# specific language governing permissions and limitations
# under the License.
#
-->
# Cordova-lib Release Notes

### 0.21.8 (Aug 29, 2014)
* CB-5535: Remove "--arc" from ios platform creation args
* CB-7416 Fixes file path reference when adding new source file
* CB-7416 handleInstall tests for null platformTag. removed uncalled 'hasPlatformSection' from PluginInfo.js
* Remove use of path.join for manifest.launch_path
* CB-7347 Improve cordova platform add /path/to handling
* CB-7118 (fix jshint warnings)
* CB-7114 Android: add support of min/max/target SDK to config.xml
* CB-7118 Use updated version of node-xcode
* CB-7118 iOS: add target-device and MinimumOSVersion support to config.xml
* ubuntu: support incremental builds
* ubuntu: support target-dir for resource-file
* ubuntu: use common.copyFile
* ubuntu: check icon existence
* ffos: Make author url optional
* CB-7142 Add <variable> to <feature> for "plugin restore" command
* Set git clone depth to 10 for Travis to make it faster
* windows: update as per changed manifest file names
* Don't spy and expect it to call the other spy ...
* Well that looks like an error
* Fixing failing tests: update_proj should be update_project
* Fix failing tests. update_jsproj and update_csproj are now just update_proj
* Fix jshint errors in amazon_fireos_parser : mixed single/double quotes
* CB-6699 Include files from www folder via single element (use ** glob pattern)
* Allow plugin modules to be .json files
* Taking care of dashes in amazon-fireos platform name.
* Upleveled amazon-fireos changes.
* Fix link/copy parent check for windows
* Style fixes - comments
* Fix error in comments for munge functions
* Add link to BuildBot at ci.cordova.io in README
* CB-7255 Fixed writing plist unescaped
* Style fixes - white space only
* Add JSCS config file
* CB-7228: Fixed issue with "cordova prepare --browserify"
* CB-7001: Create a --browserify option for run action
* CB-7228: Cordova prepare --browserify runs on all installed plugins
* CB-7190: Add browserify support in cordova-lib/cordova-cli
* CB-7260 Get cordova-android 3.5.1 instead of 3.5.0
* CB-7001: Create a --browserify option for run action
* CB-7228: Cordova prepare --browserify runs on all installed plugins
* CB-7190: Add browserify support in cordova-lib/cordova-cli
* CB-7234 added better outputs for plugin registry workflows
* CB-7100: Use npm based lazy-load by default
* CB-7091: Remove check_requirements() funcs from platform parsers
* CB-7091: Remove check_requirements() funcs from platform parsers
* CB-7140 Check plugin versions in local search path
* small refactor for missing code block after conditional statement
* CB-7203 isRelativePath needs to pass path through
* CB-7199 control git/npm using platform.js
* CB-7199 control git/npm using platform.js
* Fix style errors - make jshint happy
* CB-6756 Adds save and restore command for platforms.
* Add VERSION files to fix failing tests (forgot to git add in b7781cb)
* CB-7132 Fix regression regarding default resources
* CB-7187 Make CoreLocation a required library only for cordova-ios < 3.6.0
* Add AppVeyor badge to README
* Add Travis and npm badges to README.md
* fix(tests): cordova/lazy_load spec on Windows
* Fix plugman/install spec
* build configuration for AppVeyor
* build configurations for Travis
* CB-7124 Wrap the cordova platform string in Platform object
* CB-7140: Switch to using PluginInfo in plugman/fetch.js
* Minor style fixes in fetch.js
* CB-7078: Disable serve.spec.js
* CB-6512: platform add <path> was using wrong www/cordova.js
* CB-7083 Missing SDKReference support on Windows Phone
* CB-6874 Consolidate <Content> tag additions into 1 ItemGroup
* CB-7100: Use npm based lazy-load by default
* CB-7091: Remove check_requirements() funcs from platform parsers
* CB-7091: Don't call check_requirements during platform add
* Fix typo in comment.
* CB-7087 Retire blackberry10/ directory
* CB-6776: Fix uri/url renaming bug
* Remove npm-shrinkwrap.json


### 0.21.4 (Jun 23, 2014)
* CB-3571, CB-2606: support for splashscreens
* CB-6976 Add support for Windows Universal apps (Windows 8.1 and WP 8.1)
* Use Plugininfo module to determine plugin id and version
* Fix plugin check error, when plugin dependency with specific version is given
* CB-6709 Do not create merges/ folder when adding a platform
* CB-6140 Don't allow deletion of platform dependencies
* CB-6698: Fix 'android update lib-project' to work with paths containing spaces
* CB-6973: Run JSHint on all code in src/ via npm test
* CB-6542: Delay creating project until there's some chance that it will succeed
* folder_contents() now ignores .svn folders
* CB-6970 Share win project files manipulation code between cordova and plugman
* CB-6954: Share events.js between cordova and plugman
* CB-6698 Automatically copy sub-libraries to project's directory
* Revert "CB-6698 Resolve android <framework> relative to plugin_dir when custom=true"
* CB-6942 Describe running hooks only in verbose mode.
* CB-6512: Allow "cordova platform add /path/to/platform/files"
* Update hooks-README.md - shebang line in hooks on Windows.
* CB-6895 Add more config properties into manifest
* Allow "cordova platform add platform@version"
* Add util func for chaining promises
* removing doWrap from prepare
* adding configurable attribute
* cleaning up plugman.js for uninstall
* adding param to uninstall
* adding support for prepare flag
* adding prepare-browserify
* adding options to prepare
* adding and freezing cordova-js
* [CB-6879] config parser breakout into a cordova level module
* CB-6698 Resolve android <framework> relative to plugin_dir when custom=true
* Fix tests on node 0.11.x
* Fix android <framework> unit tests to not expect end of line.
* CB-6024: Accept cli vars as part of opts param
* Refer properties-parser package from NPM.
* CB-6859 Removed all wp7 references, tests still passing
* Extract AndroidProject class into a separate .js file
* CB-6698: Support library references for Android via the framework tag
* CB-6854 Strip BOM when adding cordova.define() to js-modules
* Add npm cache based downloading to lazy_load
* Use PluginInfo in plugman/install.js
* Extend PluginInfo to parse more of plugin.xml
* CB-6772 Provide a default for AndroidLaunchMode
* CB-6711: Use parseProjectFile when working with XCode projects.
* Start using PluginInfo object in plugman/install.js
* CB-6709 Remove merges/ folder for default apps
* support for shrinkwrap flag
* Initial implementation for restore and save plugin
* CB-6668: Use <description> for "plugin ls" when <name> is missing.
* Add --noregstry flag for disabling plugin lookup in the registry
* Remove --force from default npm settings for plugin registry
* Use "npm info" for fetching plugin metadata
* Use "npm cache add" for downloading plugins
* CB-6691: Change some instances of Error() to CordovaError()


### 0.21.1
Initial release v0.21.1 (picks up from the same version number as plugman was).
