This is the Grails Resources framework.

NB: The tests do not run, there appears to be a weird bug in Grails that causes the tagLib that runs the tests to not be the one
created in the ResourceTagLibTests - and the injected services are missing.

It provides a DSL for declaring static resources in plugins and in apps, and a mapper artefact that allows other plugins to provide processing of static resources to e.g. minify / zip them.

All processing is performed at runtime once, against files in the server filesystem.

Built-in mappers included in the plugin:

* CSS rewriter (two mappers required, happens automatically)
* Bundler (combines multiple css or js files into one)

See docs at http://grails.org/plugin/resources
