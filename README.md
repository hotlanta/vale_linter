Vale is a grammar, style, and word usage linter for the English language. Vale’s configuration needs to be stored in the .vale.ini file located in the root directory of a project. The styles folder should also be stored in the root directory of a project.

The Vale files in this repo implement the HPE style guide.

To check a file(s) the following command can be used in CLI:
vale file._ file._ ...

1. [Vale installation instructions](https://docs.errata.ai/vale/install) -- <b>Note: Run Windows Powershell as an Admin!</b>

    - Copy [Vale styles folder](https://github.com/hotlanta/vale_linter/tree/main/styles) to your local repo and modify as needed. The styles found here are based on the HPE style guide, plus spell checker,, spelling exceptions, and some common sense styles (base folder).
    
    - Copy [.vale.ini](https://github.com/hotlanta/vale_linter/blob/main/.vale.ini) file to your local repo and modify as needed.

2. [Online tool for building Vale rules](https://github.com/errata-ai/vale-studio) -- Use if you need to create or update \*.yml files to check for additional conditions.

3. Editing Environment Variable -- under the "Path" variable add the paths to the necessary Vale files

- Example:

  ![env_var_1](https://github.com/hotlanta/vale_linter/blob/main/images/environment_variables.png)

4. Installing Vale on VS Code

- install vale-vscode via [Marketplace](https://marketplace.visualstudio.com/items?itemName=errata-ai.vale-server)
- set [vale.core.useCLI](https://github.com/errata-ai/vale-vscode#settings) to true in the extension settings (Preferences > Extensions > Vale > Use CLI)
- restart VS Code (recommended).
- go to Extensions -> Vale -> Settings and complete the settings for using CLI and indicating where your .vale.ini and vale.exe files are located.

  Example:
  ![vscode_config_1](https://github.com/hotlanta/vale_linter/blob/main/images/vscode_config_1.png)
  ![vscode_config_2](https://github.com/hotlanta/vale_linter/blob/main/images/vscode_config_2.png)

5. [Integration with Atom text editor](https://atom.io/packages/atomic-vale)

6. [Vale usage with a continuous integration (CI) service](https://docs.errata.ai/vale/install#using-vale-with-a-continuous-integration-ci-service)

7. Integration with Oxygen Author XML terminology checker add-on [(Installation instructions)](https://www.oxygenxml.com/doc/versions/23.1/ug-editor/topics/terminology-checker-addon.html)

- Add the terminology checker file to the folder containing your Vale linter \*.yml files
  ![term_checker_1](https://github.com/hotlanta/vale_linter/blob/main/images/terminology_checker_file.png)
- Select the correct Terminology folder: Preferences->Plugins->Terminology Checker
  ![term_checker_2](https://github.com/hotlanta/vale_linter/blob/main/images/terminology_checker.png)
- Note that Oxygen Author XML will have some error messages from using the Vale _.yml files. These error messages are the because only certain _.yml files are supported. These error messages can be ignored. The following type of Vale \*yml files are supported:

  - Supported Vale scopes: heading, table.header, table.cell, list, paragraph, code, strong, emphasis.
  - Supported Vale extension points: Existence, Substitution, Occurrence.

8. For further usage and automation, see [Vale linter wiki](https://github.com/hotlanta/vale_linter/wiki)!

9. References
    - styles used were based on yaml styles that can be found in these locations (note that some styles have been modified from their original version):    
        - https://github.com/topics/vale-linter-style        
        - https://github.com/errata-ai/styles
