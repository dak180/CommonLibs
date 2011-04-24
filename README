CommonLibs
	A collection of Xcode project files to download and build libraries as frameworks.


Overview
	These Xcode projects each build a single lib; they are meant to be included in larger projects.

	They work by downloading a copy of source for the lib at build time and produce a framework suitable for use in Mac applications.

	As much as possible has been externalized from the Xcode project files to make for easier merging and to give you a better idea how they work.


Specifications
	All libs have the following configurations: Release, Debug and StaticAnalyzer (an alias of Debug); they will by default build in the Release configuration.

	All libs are Universal Binaries with the following architectures: ppc, i386 and x86_64.  The 32 bit architectures are built against the 10.5 sdk with a deployment target of 10.4; the x86_64 architecture is built against the 10.6 sdk with a deployment target of the same.


Structure
	Each lib uses the following files:
		configs/Base-All.xcconfig
		configs/Base.xcconfig
		configs/FetchPrebuilt.sh
		configs/FetchSource.sh
		configs/{LibName}-All.xcconfig
		configs/{LibName}-Debug.xcconfig
		configs/{LibName}-Release.xcconfig
		{LibName}.xcodeproj/project.pbxproj
		Resources/GenericFramework-Info.plist

	The following directories and their contents will be created and managed at build time (not all of these may be used by every lib):
		build
		external
		prebuilt
