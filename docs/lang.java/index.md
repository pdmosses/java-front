---
hide:
  - toc
---

# Java Front

:simple-github: [pdmosses/java-front/README]

[metaborgcube/java-front/README]: https://github.com/metaborgcube/java-front/blob/master/README.md "The original file on GitHub"

> A declarative specification of Java 8's syntax in [Spoofax].

## Syntax

[`metaborg-java.sdf3`](syntax/metaborg-java.sdf3.md)

This example demonstrates generation of a hyperlinked twin from
an [SDF3] definition of the syntax of a major programming language.

## Name binding

The name binding of Java has not yet been specified in Spoofax meta-languages.

## Project Structure

> Each subdirectory of `syntax/java` contains specifications for a section of the Java language:

> * arrays  - Syntax for array initializers
> * classes - Class, method, constructor, field and enum declarations
> * expressions - All expressions
> * interfaces - Interface, abstract method, constant and annotation declarations
> * lexical - Lexical syntax for identifiers, comments, layout, etc.
> * literals - Boolean, numerical, string, and null literals
> * names - References to definitions of names
> * packages - Compilation unit, package, and import declarations
> * statements - All statements
> * types - Primitive and reference types

> The project also contains tests with Java files from the Spoofax codebase,
and succeeding tests from the Java language specification.

[Spoofax]: https://spoofax.dev
[SDF3]: https://spoofax.dev/references/sdf3/
