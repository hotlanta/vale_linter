# asciidoc-authoring.md

## Purpose

Use this skill whenever creating or modifying AsciiDoc documentation.

The goal is to produce content that complies with organizational writing standards and avoids common validation failures.

---

# Headings

Use sentence case for all headings.

Good:

```adoc
== Configure the gateway
```

Bad:

```adoc
== Configure The Gateway
== CONFIGURE THE GATEWAY
```

Rules:

* The first word begins with a capital letter.
* Subsequent words should normally be lowercase unless they are proper nouns, product names, acronyms, or trademarks.

---

# Tables and images

Every table must have a title.

Good:

```adoc
.Table 1. Configuration parameters
|===
...
|===
```

Every image must have a title.

Good:

```adoc
.Image 1. Login page
image::login.png[Login page]
```

Do not create untitled tables or images.

---

# Lists

Do not create lists containing only a single item.

Instead of:

```adoc
* Configure the server.
```

Write a normal paragraph.

---

# List consistency

Avoid mixing sentence-style and fragment-style list items.

Bad:

```adoc
* Configure the server
* The service starts automatically.
* Verify connectivity
```

Good:

```adoc
* Configure the server.
* Start the service.
* Verify connectivity.
```

or

```adoc
* Server configuration
* Service startup
* Connectivity verification
```

If any item ends with a period, all items should end with a period.

---

# Short descriptions

Every topic should begin with a concise introductory description.

Guidelines:

* Maximum 50 words.
* Explain the purpose of the topic.
* Avoid marketing language.
* Avoid repeating the title.

Example:

```adoc
This procedure describes how to configure the gateway service.
```

---

# Whitespace

Avoid unnecessary whitespace.

Rules:

* No double spaces between words.
* No trailing spaces.
* No leading spaces.
* Do not leave blank inline formatting elements.

Bad:

```adoc
This  sentence has  extra spaces.
```

Bad:

```adoc
` command `
```

Good:

```adoc
`command`
```

---

# Inline formatting

Do not place spaces immediately inside inline formatting.

Bad:

```adoc
` command `
* text *
```

Good:

```adoc
`command`
*text*
```

---

# Numbers

Spell out numbers from zero through nine when used in running text.

Good:

```adoc
Configure three servers.
```

Bad:

```adoc
Configure 3 servers.
```

Exceptions:

* Tables
* Mathematical expressions
* Measurements
* Product version numbers
* Commands and code

---

# Commas before conjunctions

When joining items in a series, place a comma before:

* and
* or
* but

Good:

```adoc
Install the package, configure the service, and restart the server.
```

Good:

```adoc
Use TCP, UDP, or SCTP.
```

---

# Links

Do not use raw URLs as link text.

Bad:

```adoc
https://example.com
```

Bad:

```adoc
link:https://example.com[https://example.com]
```

Good:

```adoc
link:https://example.com[Gateway configuration guide]
```

Link text should describe the destination.

---

# Images

Do not use automatic image scaling.

Avoid:

```adoc
image::example.png[]
```

Specify dimensions explicitly when needed.

Example:

```adoc
image::example.png[width=600]
```

---

# Tables

Use proportional column widths.

Good:

```adoc
[cols="2*,1*,3*"]
|===
...
|===
```

Avoid fixed-width column definitions whenever possible.

---

# Content completeness

Do not leave content placeholders or empty elements.

Every section should contain meaningful content.

Avoid:

* Empty paragraphs
* Empty notes
* Empty list items
* Empty code blocks
* Empty titles

---

# Metadata

Every topic should contain maintenance metadata.

Include:

* Author
* Product name
* Version information
* Revision date

Use ISO date format:

```text
YYYY-MM-DD
```

Example:

```text
2026-06-16
```

---

# Cross-references

When creating internal cross-references:

* Verify that the target exists.
* Verify that anchors are valid.
* Verify that links point to the correct section.

Do not create references to content that does not exist.

---

# General writing principles

Before completing a document:

1. Verify all headings use sentence case.
2. Verify every image has a title.
3. Verify every table has a title.
4. Verify lists contain more than one item.
5. Verify no extra whitespace exists.
6. Verify numbers below ten are spelled out.
7. Verify link text describes the destination.
8. Verify all cross-references resolve correctly.
9. Verify metadata is present and current.
10. Verify no section is empty.

```
```
