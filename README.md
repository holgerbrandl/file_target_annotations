> file annotations have to be on top of everything, just switch places between your annotation and package


![](.README_images/1af75ba8.png)

It seems to work only for stdlb annotations and not for annotations added via classpath. IJ seems aware of the existence because it’s showing an import popup, but there should be no need to import since the `DependsOn` annotation is declared on toplevel as is

This repo contains a SSCE to illustrate the issue.
