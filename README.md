

Sometimes you want to connect your favorite database visualzation tool to Hive.  I've found that this can be somewhat cumbersome, typically requireing you to copy jars from the distro to some place locally that can be read by your tool.  The goal of this simple maven project was to easily pull the required jars into a single place locally and create an "uber" jar that can be referenced by any JDBC hungry tool.

To get started you must have Maven installed locally.  After that its a simple as running `mvn:package`.  A file called `hive-jdbc-uber-1.0.jar` will be created in your `target` directory.  After that point your favorite tool to this jar.  It will have the necessary Hive JDBC drivers as well as required dependencies.
