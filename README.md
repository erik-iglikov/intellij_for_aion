# IntelliJ IDEA support for the Aion project

The only purpose for this repository is to make it easy to import the [Aion project](https://github.com/aionnetwork/aion) into IntelliJ IDEA.

To get started first clone the Aion project. Make sure to add the `--recursive` option when cloning or initialize the submodules after cloning.

Next, clone this project into a separate folder.

Then run the commands:
```
rm -fr intellij_for_aion/.git intellij_for_aion/README.md intellij_for_aion/UpdateScript.sh
rsync -rv intellij_for_aion/ aion/
```
where `aion` contains the code base and `intellij_for_aion` contains the IDE support files.

IntelliJ IDEA should now be able to open the project and view the modules and dependencies.

**Note:** I am making no guarantees on keeping the .iml files up to date ;)
