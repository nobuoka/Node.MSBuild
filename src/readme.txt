Node.MSBuild
====================

* This project provides MSBuild target `SetupNode`, and it is included in a `BuildDependsOn` property.
* Changing the version of Node.js to be installed, set the version as the value of MSBuild property `NodeVersion`.
    * For example: `<NodeVersion>5.2.0</NodeVersion>`.
* Executing `node` command, use `Exec` task with `NodeCommand` property:
    * For example: `<Exec Command="$(NodeCommand) foo\bar.js " />`.
