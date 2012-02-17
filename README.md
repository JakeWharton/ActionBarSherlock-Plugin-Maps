ActionBarSherlock Plugin: Maps
==============================

Plugin for [ActionBarSherlock][1] which provides a base activity that can be
used for adding a `MapView` to your action bar-enabled layouts.

*Note:* This does not provide support for placing a `MapView` in fragments.



Compilation
-----------

*Compilation requires that you have deployed the Google APIs corresponding to
API 14 using the [maven-android-sdk-deployer][2].*

`mvn clean verify` and you're done.

The plugin will be in `plugin/target/` and a sample APK will be in
`sample/target/`



Including In Your Project
-------------------------

This library is presented as a `.jar` file which you can include in the `libs/`
folder of your application. You can download the latest version from the
[GitHub downloads page][3].

In order to use the plugin you must already have referenced the main
[ActionBarSherlock][1] library in your project. You will also be required to
compile your project with the appropriate Google APIs to use this plugin.

If you are a Maven user you can easily include the library by specifying it as
a dependency:

    <dependency>
      <groupId>com.actionbarsherlock</groupId>
      <artifactId>plugin-maps</artifactId>
      <version><!-- LATEST PLUGIN VERSION --></version>
    </dependency>

Since the Google Maps APIs are not available in central this plugin is deployed
to Jake Wharton's personal repository. You can add it with the following:

    <repository>
      <id>com.jakewharton</id>
      <url>http://r.jakewharton.com/maven/release</url>
    </repository>





 [1]: http://actionbarsherlock.com
 [2]: https://github.com/mosabua/maven-android-sdk-deployer
