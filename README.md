
> file annotations have to be on top of everything, just switch places between your annotation and package


It seems to work only for stdlb annotations and not for annotations added via classpath.

This repo contains a SSCE to illustrate the issue.

```bash
gradle build
```

gives
```
e: /Users/brandl/projects/kotlin/misc/file_pckg_annot/src/main/kotlin/com/foobar/WithPckg.kt: (2, 7): Unresolved reference: MyAnno

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':compileKotlin'.
> Compilation error. See log for more details

* Try:
Run with --stacktrace option to get the stack trace. Run with --info or --debug option to get more log output.

* Get more help at https://help.gradle.org

BUILD FAILED in 0s
1 actionable task: 1 executed

```

IJ is also not able to process it correctly:

![](.README_images/9c980a0f.png)

