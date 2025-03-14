# CMake 学习手册
&nbsp;&nbsp;文档太多，时间有限，因此，了解使用框架，各个命令的用途，详细用途后续补充.

## cmake --help
```txt
    Firmware-Engineer git:(master) cmake --help
    Usage
    
      cmake [options] <path-to-source>
      cmake [options] <path-to-existing-build>
      cmake [options] -S <path-to-source> -B <path-to-build>
    
    Specify a source directory to (re-)generate a build system for it in the
    current working directory.  Specify an existing build directory to
    re-generate its build system.
    
    Options
      -S <path-to-source>          = Explicitly specify a source directory.
      -B <path-to-build>           = Explicitly specify a build directory.
      -C <initial-cache>           = Pre-load a script to populate the cache.
      -D <var>[:<type>]=<value>    = Create or update a cmake cache entry.
      -U <globbing_expr>           = Remove matching entries from CMake cache.
      -G <generator-name>          = Specify a build system generator.
      -T <toolset-name>            = Specify toolset name if supported by
                                     generator.
      -A <platform-name>           = Specify platform name if supported by
                                     generator.
      --toolchain <file>           = Specify toolchain file
                                     [CMAKE_TOOLCHAIN_FILE].
      --install-prefix <directory> = Specify install directory
                                     [CMAKE_INSTALL_PREFIX].
      -Wdev                        = Enable developer warnings.
      -Wno-dev                     = Suppress developer warnings.
      -Werror=dev                  = Make developer warnings errors.
      -Wno-error=dev               = Make developer warnings not errors.
      -Wdeprecated                 = Enable deprecation warnings.
      -Wno-deprecated              = Suppress deprecation warnings.
      -Werror=deprecated           = Make deprecated macro and function warnings
                                     errors.
      -Wno-error=deprecated        = Make deprecated macro and function warnings
                                     not errors.
      --preset <preset>,--preset=<preset>
                                   = Specify a configure preset.
      --list-presets               = List available presets.
      -E                           = CMake command mode.
      -L[A][H]                     = List non-advanced cached variables.
      --build <dir>                = Build a CMake-generated project binary tree.
      --install <dir>              = Install a CMake-generated project binary
                                     tree.
      --open <dir>                 = Open generated project in the associated
                                     application.
      -N                           = View mode only.
      -P <file>                    = Process script mode.
      --find-package               = Legacy pkg-config like mode.  Do not use.
      --graphviz=[file]            = Generate graphviz of dependencies, see
                                     CMakeGraphVizOptions.cmake for more.
      --system-information [file]  = Dump information about this system.
      --log-level=<ERROR|WARNING|NOTICE|STATUS|VERBOSE|DEBUG|TRACE>
                                   = Set the verbosity of messages from CMake
                                     files.  --loglevel is also accepted for
                                     backward compatibility reasons.
      --log-context                = Prepend log messages with context, if given
      --debug-trycompile           = Do not delete the try_compile build tree.
                                     Only useful on one try_compile at a time.
      --debug-output               = Put cmake in a debug mode.
      --debug-find                 = Put cmake find in a debug mode.
      --trace                      = Put cmake in trace mode.
      --trace-expand               = Put cmake in trace mode with variable
                                     expansion.
      --trace-format=<human|json-v1>
                                   = Set the output format of the trace.
      --trace-source=<file>        = Trace only this CMake file/module.  Multiple
                                     options allowed.
      --trace-redirect=<file>      = Redirect trace output to a file instead of
                                     stderr.
      --warn-uninitialized         = Warn about uninitialized values.
      --no-warn-unused-cli         = Don't warn about command line options.
      --check-system-vars          = Find problems with variable usage in system
                                     files.
      --profiling-format=<fmt>     = Output data for profiling CMake scripts.
                                     Supported formats: google-trace
      --profiling-output=<file>    = Select an output path for the profiling data
                                     enabled through --profiling-format.
      --help,-help,-usage,-h,-H,/? = Print usage information and exit.
      --version,-version,/V [<f>]  = Print version number and exit.
      --help-full [<f>]            = Print all help manuals and exit.
      --help-manual <man> [<f>]    = Print one help manual and exit.
      --help-manual-list [<f>]     = List help manuals available and exit.
      --help-command <cmd> [<f>]   = Print help for one command and exit.
      --help-command-list [<f>]    = List commands with help available and exit.
      --help-commands [<f>]        = Print cmake-commands manual and exit.
      --help-module <mod> [<f>]    = Print help for one module and exit.
      --help-module-list [<f>]     = List modules with help available and exit.
      --help-modules [<f>]         = Print cmake-modules manual and exit.
      --help-policy <cmp> [<f>]    = Print help for one policy and exit.
      --help-policy-list [<f>]     = List policies with help available and exit.
      --help-policies [<f>]        = Print cmake-policies manual and exit.
      --help-property <prop> [<f>] = Print help for one property and exit.
      --help-property-list [<f>]   = List properties with help available and
                                     exit.
      --help-properties [<f>]      = Print cmake-properties manual and exit.
      --help-variable var [<f>]    = Print help for one variable and exit.
      --help-variable-list [<f>]   = List variables with help available and exit.
      --help-variables [<f>]       = Print cmake-variables manual and exit.
    
    Generators
    
    The following generators are available on this platform (* marks default):
    * Unix Makefiles               = Generates standard UNIX makefiles.
      Ninja                        = Generates build.ninja files.
      Ninja Multi-Config           = Generates build-<Config>.ninja files.
      Watcom WMake                 = Generates Watcom WMake makefiles.
      Xcode                        = Generate Xcode project files.
      CodeBlocks - Ninja           = Generates CodeBlocks project files.
      CodeBlocks - Unix Makefiles  = Generates CodeBlocks project files.
      CodeLite - Ninja             = Generates CodeLite project files.
      CodeLite - Unix Makefiles    = Generates CodeLite project files.
      Eclipse CDT4 - Ninja         = Generates Eclipse CDT 4.0 project files.
      Eclipse CDT4 - Unix Makefiles= Generates Eclipse CDT 4.0 project files.
      Kate - Ninja                 = Generates Kate project files.
      Kate - Unix Makefiles        = Generates Kate project files.
      Sublime Text 2 - Ninja       = Generates Sublime Text 2 project files.
      Sublime Text 2 - Unix Makefiles
                                   = Generates Sublime Text 2 project files.
```
    