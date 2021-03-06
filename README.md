# AltiumDesignerResource

This repossitory is a collection of useful templates I created for Altium Designer.

The subfolders are described as following:

| Folder           |                                                 Description |
| ---------------- | ----------------------------------------------------------: |
| BOM              | Excel templates which will be called from the outjob script |
| LayerTemplates   |  Templates for layerstacks to be imported into new projects |
| ProjectTemplates |         Basic project templates to accelerate project start |
| RuleTemplates    |          Rule template which can be imported into a project |

## ProjectTemplates

I use Altiums "special-strings" to organize my projects, the projects version and revision and also the automated manufacturing outputs.
Thats why I added the following strings to my projects in (Altium > Project > Project Options > Parameters (Tab)).

| String           |                 Description |
| ---------------- | --------------------------: |
| mCompanyAddress  |             Company Address |
| mCompanyName     |        Name of your company |
| mCompanyStreet   |           Company address 2 |
| mProjectAuthor   | Name of the projects author |
| mProjectName     |         Name of the project |
| mProjectRevision |  Project revision (eq. X.2) |
| mProjectVersion  |   Project version (eq. 1.X) |

You can easy access those special strings from Schematic, using "=" sign (eq. =mProjectName) or in pcb view using "." sign (eq. .mProjectName). The main benefit of this approach is that you only have one place where you need to change the name or the version. If you update your board and version you only need to change the special string value in your project options. It is unique for your project and easy and fast to handle. You can also use it to organize the manufacturing outputs of gerber, drill or BOM/CSV files etc. By adding the special strings to the generated output name it is possible to ensure the correct version of your project.

The projects also come with the variant "Default" to support the outjob file structure. The schematic and pcb templates are in a A3 and A4 version. When starting the project with those templates you can simply choose the one that fits your board size, rename them and remove the other one. The pcb doc files are optimized for printing with a scale of 1.00 for A3 and A4. Documenation is on ML7.

## OutJob

...

### Disclaimer

These examples are provided as-are, and there are no guarantees that they fit your purposes or that they are bug-free. Use it at your own risk! The resources and libraries may provide 3D data, scripts footprints or schematic files from third parties with or without copyrights.
