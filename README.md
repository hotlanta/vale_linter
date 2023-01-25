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

   c. GitHub actions is another method of automation: [Vale GitHub action](https://github.com/errata-ai/vale-action). It has to be enabled by writing this email address - scm_ghe_admins@groups.ext.hpe.com - to ask the admins to enable it for your repo.

5. [Understanding the Vale command line tool output](https://github.hpe.com/eric-szegedi/vale_linter/wiki/Understanding-the-Vale-command-line-tool-output)

6. References

   Rules used to convert the HPE Style Guide were based on YAML styles that can be found in these locations:

   **Note** Some styles have been modified from their original version.

   - <https://github.com/topics/vale-linter-style>
   - <https://github.com/errata-ai/styles>

7. Upgrade Vale

   If Vale was installed on your machine using the `choco` command, then to update Vale to a new release run the command `choco upgrade vale`.

8. Extension points

| **Check**                                                       | **Implementations** |
|-----------------------------------------------------------------|---------------------|
| [existence](https://errata-ai.github.io/vale/styles/#existence) | HPE: AM_PM.yml, Ampersands, Begin_sentence.yml, But.yml, Capitalize_file_extensions.yml, Dates_ordinal.yml, Dates.yml, Directional_language.yml, Disabilities.yml, EmDash.yml, EnDash.yml, Ensure.yml, Exclamation.yml, Heading_capitalization.yml, headingPunctuation.yml, HPE_a_an.yml, HPE_Ellipses.yml, HPE_hyphen.yml, Indefinite_modifiers.yml, Jargon.yml, MeaningfulLinkWords.yml, MeaningfulWords_colors_shapes.yml, Negative_numbers.yml, Numbers_ranges.yml, Numeric_dates, Passive.yml, Person.yml, Prepositions_end_sentence.yml, Prepositions.yml, Quote_punctuation.yml, Semicolons.yml, Slash.yml, Spaces.yml, Tense.yml, Time_ranges.yml, Units_space, Wordiness,yml <br/><br/> Base: Capitalize_list_start.yml, Customer_names.yml, Empty_reference.yml, So.yml, Validate_wordiness.yml |
| [substitution](https://errata-ai.github.io/vale/styles/#substitution) | HPE: 24_7.yml, above_below.yml, Advice_advise.yml, Appendixes, HPE_Avoid.yml, Backup.yml, British.yml, Contractions.yml, End_user.yml, Gender.yml, HPE_name.yml, HPE_possessive.yml, InclusionCultural.yml, InclusionOther.yml, Latin.yml, Logon_login.yml, Noon_midnight.yml, Numbers.yml, Please.yml, Positive.yml, Pull_down.yml, Redundant.yml, Setup.yml, Should.yml, Terms_ignorecase_false.yml, Terms_ignorecase_true.yml, Very.yml, Word_choice.yml, Zero.yml <br/><br/> Base: Backend.yml, Term_Consistency_yml, Typography.yml  |
| [occurrence](https://errata-ai.github.io/vale/styles/#occurrence) | Commas_morethanthree.yml, Sentence_length.yml |
| [repetition](https://errata-ai.github.io/vale/styles/#repetition) | Repetition.yml |
| [consistency](https://errata-ai.github.io/vale/styles/#consistency) | Consistency.yml |
| [capitalization](https://errata-ai.github.io/vale/styles/#capitalization) | Capitalization.yml |
| [readability](https://errata-ai.github.io/vale/styles/#readability) | N/A |
| [conditional](https://errata-ai.github.io/vale/styles/#conditional) | HPE: Acronyms_abbreviations.yml  <br/><br/> Base: UnexpandedAcronyms.yml |
| [spelling](https://errata-ai.github.io/vale/styles/#spelling) | Spelling.yml |
