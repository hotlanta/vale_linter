Vale is a grammar, style, and word usage linter for the English language. Vale’s configuration needs to be stored in the .vale.ini file located in the root directory of a project. The styles folder can be referenced by an absolute path or a relative path.

**The Vale files in this repo implement the HPE style guide.**

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

The following points below provide installation instructions, setup and configuration steps, details and links for using various interfaces with Vale, and a link for automating the running of Vale with GitHub.

1. [Installation and system configuration](https://github.hpe.com/eric-szegedi/vale_linter/wiki/Vale-linter-installation-and-system-configuration)
  
2. [Integrating with other interfaces to work with Vale](https://github.hpe.com/eric-szegedi/vale_linter/wiki/Vale-integration-with-other-interfaces)

3. [Usage](https://github.hpe.com/eric-szegedi/vale_linter/wiki/Vale-usage) and [creation of new Vale linter rules](https://github.com/errata-ai/vale-studio)

4. Review automation with lefthook

   a. [Vale review automation with `git push` and lefthook](https://github.hpe.com/eric-szegedi/vale_linter/wiki/Automating-Vale-linter-checks-with-lefthook)

   b. [Vale usage with a continuous integration (CI) service](https://docs.errata.ai/vale/install#using-vale-with-a-continuous-integration-ci-service)

   c. Whenever HPE GitHub Enterprise enables GitHub actions, then this can be another method of automation: [Vale GitHub action](https://github.com/errata-ai/vale-action). Until then only #1 and # 2 review automation tools can be used.

5. References

   Rules used to convert the HPE Style Guide were based on YAML styles that can be found in these locations:

   **Note** Some styles have been modified from their original version.

   - <https://github.com/topics/vale-linter-style>
   - <https://github.com/errata-ai/styles>
