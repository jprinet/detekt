---
title: Formatting Rule Set
sidebar: home_sidebar
keywords: [rules, formatting]
permalink: formatting.html
toc: true
folder: documentation
---
This rule set provides wrappers for rules implemented by ktlint - https://ktlint.github.io/.

Note: Issues reported by this rule set can only be suppressed on file level (`@file:Suppress("detekt.rule")`).
Note: The formatting rule set is not included in the detekt-cli or gradle plugin.

To enable this rule set, add `detektPlugins "io.gitlab.arturbosch.detekt:detekt-formatting:$version"`
to your gradle dependencies or reference the `detekt-formatting`-jar with the `--plugins` option
in the command line interface.

### AnnotationOnSeparateLine

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#annotation-formatting) for documentation.

**Active by default**: Yes - Since v1.22.0

### AnnotationSpacing

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#annotation-spacing) for documentation.

**Active by default**: Yes - Since v1.22.0

### ArgumentListWrapping

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#argument-list-wrapping) for documentation.

**Active by default**: Yes - Since v1.22.0

#### Configuration options:

* ``indentSize`` (default: ``4``)

  indentation size

* ``maxLineLength`` (default: ``120``) (android default: ``100``)

  maximum line length

### BlockCommentInitialStarAlignment

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#block-comment-initial-star-alignment) for
documentation.

**Active by default**: No

### ChainWrapping

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#chain-wrapping) for documentation.

**Active by default**: Yes - Since v1.0.0

### CommentSpacing

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#comment-spacing) for documentation.

**Active by default**: Yes - Since v1.0.0

### CommentWrapping

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#comment-wrapping) for documentation.

**Active by default**: No

#### Configuration options:

* ``indentSize`` (default: ``4``)

  indentation size

### DiscouragedCommentLocation

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#discouraged-comment-location) for
documentation.

**Active by default**: No

### EnumEntryNameCase

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#enum-entry) for documentation.

**Active by default**: Yes - Since v1.22.0

### Filename

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#file-name) for documentation.

This rules overlaps with [naming&gt;MatchingDeclarationName](https://detekt.dev/naming.html#matchingdeclarationname)
from the standard rules, make sure to enable just one.

**Active by default**: Yes - Since v1.0.0

### FinalNewline

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#final-newline) for documentation.

This rules overlaps with [style&gt;NewLineAtEndOfFile](https://detekt.dev/style.html#newlineatendoffile)
from the standard rules, make sure to enable just one. The pro of this rule is that it can auto-correct the issue.

**Active by default**: Yes - Since v1.0.0

#### Configuration options:

* ``insertFinalNewLine`` (default: ``true``)

  report absence or presence of a newline

### FunKeywordSpacing

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#fun-keyword-spacing) for documentation.

**Active by default**: No

### FunctionReturnTypeSpacing

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#function-return-type-spacing) for
documentation.

**Active by default**: No

### FunctionSignature

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#function-signature) for
documentation.

**Active by default**: No

#### Configuration options:

* ``forceMultilineWhenParameterCountGreaterOrEqualThan`` (default: ``2147483647``)

  parameter count means multiline threshold

* ``functionBodyExpressionWrapping`` (default: ``'default'``)

  indentation size

* ``maxLineLength`` (default: ``120``) (android default: ``100``)

  maximum line length

* ``indentSize`` (default: ``4``)

  indentation size

### FunctionStartOfBodySpacing

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#function-start-of-body-spacing) for
documentation.

**Active by default**: No

### FunctionTypeReferenceSpacing

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#function-type-reference-spacing) for
documentation.

**Active by default**: No

### ImportOrdering

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#import-ordering) for documentation.

For defining import layout patterns see the [KtLint Source Code](https://github.com/pinterest/ktlint/blob/a6ca5b2edf95cc70a138a9470cfb6c4fd5d9d3ce/ktlint-ruleset-standard/src/main/kotlin/com/pinterest/ktlint/ruleset/standard/ImportOrderingRule.kt)

**Active by default**: Yes - Since v1.19.0

#### Configuration options:

* ``layout`` (default: ``'*,java.**,javax.**,kotlin.**,^'``) (android default: ``'*'``)

  the import ordering layout

### Indentation

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#indentation) for documentation.

**Active by default**: Yes - Since v1.19.0

#### Configuration options:

* ``indentSize`` (default: ``4``)

  indentation size

* ~~``continuationIndentSize``~~ (default: ``4``)

  **Deprecated**: `continuationIndentSize` is ignored by KtLint and will have no effect

  continuation indentation size

### KdocWrapping

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#kdoc-wrapping) for documentation.

**Active by default**: No

#### Configuration options:

* ``indentSize`` (default: ``4``)

  indentation size

### MaximumLineLength

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#max-line-length) for documentation.

This rules overlaps with [style&gt;MaxLineLength](https://detekt.dev/style.html#maxlinelength)
from the standard rules, make sure to enable just one or keep them aligned. The pro of this rule is that it can
auto-correct the issue.

**Active by default**: Yes - Since v1.0.0

#### Configuration options:

* ``maxLineLength`` (default: ``120``) (android default: ``100``)

  maximum line length

* ``ignoreBackTickedIdentifier`` (default: ``false``)

  ignore back ticked identifier

### ModifierListSpacing

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#modifier-list-spacing) for documentation.

**Active by default**: No

### ModifierOrdering

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#modifier-order) for documentation.

This rules overlaps with [style&gt;ModifierOrder](https://detekt.dev/style.html#modifierorder)
from the standard rules, make sure to enable just one. The pro of this rule is that it can auto-correct the issue.

**Active by default**: Yes - Since v1.0.0

### MultiLineIfElse

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#multiline-if-else) for documentation.

**Active by default**: Yes - Since v1.22.0

### NoBlankLineBeforeRbrace

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#no-blank-lines-before) for documentation.

**Active by default**: Yes - Since v1.0.0

### NoBlankLinesInChainedMethodCalls

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#no-blank-lines-in-chained-method-calls) for
documentation.

**Active by default**: Yes - Since v1.22.0

### NoConsecutiveBlankLines

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#no-consecutive-blank-lines) for documentation.

**Active by default**: Yes - Since v1.0.0

### NoEmptyClassBody

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#no-empty-class-bodies) for documentation.

**Active by default**: Yes - Since v1.0.0

### NoEmptyFirstLineInMethodBlock

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#no-leading-empty-lines-in-method-blocks) for
documentation.

**Active by default**: Yes - Since v1.22.0

### NoLineBreakAfterElse

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#no-line-break-after-else) for documentation.

**Active by default**: Yes - Since v1.0.0

### NoLineBreakBeforeAssignment

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#no-line-break-before-assignment) for
documentation.

**Active by default**: Yes - Since v1.0.0

### NoMultipleSpaces

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#no-multi-spaces) for documentation.

**Active by default**: Yes - Since v1.0.0

### NoSemicolons

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#no-semicolons) for documentation.

**Active by default**: Yes - Since v1.0.0

### NoTrailingSpaces

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#no-trailing-whitespaces) for documentation.

**Active by default**: Yes - Since v1.0.0

### NoUnitReturn

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#no-unit-as-return-type) for documentation.

**Active by default**: Yes - Since v1.0.0

### NoUnusedImports

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#no-unused-imports) for documentation.

**Active by default**: Yes - Since v1.0.0

### NoWildcardImports

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#no-wildcard-imports) for documentation.

**Active by default**: Yes - Since v1.0.0

#### Configuration options:

* ``packagesToUseImportOnDemandProperty`` (default: ``'java.util.*,kotlinx.android.synthetic.**'``)

  Defines allowed wildcard imports

### NullableTypeSpacing

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#nullable-type-spacing) for
documentation.

**Active by default**: No

### PackageName

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#no-underscores-in-package-names) for
documentation.

**Active by default**: Yes - Since v1.22.0

### ParameterListSpacing

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#parameter-list-spacing) for
documentation.

**Active by default**: No

### ParameterListWrapping

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#parameter-list-wrapping) for documentation.

**Active by default**: Yes - Since v1.0.0

#### Configuration options:

* ``maxLineLength`` (default: ``120``) (android default: ``100``)

  maximum line length

* ~~``indentSize``~~ (default: ``4``)

  **Deprecated**: `indentSize` is ignored by KtLint and will have no effect

  indentation size

### SpacingAroundAngleBrackets

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#angle-bracket-spacing) for documentation.

**Active by default**: Yes - Since v1.22.0

### SpacingAroundColon

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#colon-spacing) for documentation.

**Active by default**: Yes - Since v1.0.0

### SpacingAroundComma

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#comma-spacing) for documentation.

**Active by default**: Yes - Since v1.0.0

### SpacingAroundCurly

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#curly-spacing) for documentation.

**Active by default**: Yes - Since v1.0.0

### SpacingAroundDot

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#dot-spacing) for documentation.

**Active by default**: Yes - Since v1.0.0

### SpacingAroundDoubleColon

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#double-colon-spacing) for documentation.

**Active by default**: Yes - Since v1.22.0

### SpacingAroundKeyword

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#keyword-spacing) for documentation.

**Active by default**: Yes - Since v1.0.0

### SpacingAroundOperators

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#operator-spacing) for documentation.

**Active by default**: Yes - Since v1.0.0

### SpacingAroundParens

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#parenthesis-spacing) for documentation.

**Active by default**: Yes - Since v1.0.0

### SpacingAroundRangeOperator

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#range-spacing) for documentation.

**Active by default**: Yes - Since v1.0.0

### SpacingAroundUnaryOperator

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#unary-operator-spacing) for documentation.

**Active by default**: Yes - Since v1.22.0

### SpacingBetweenDeclarationsWithAnnotations

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#blank-line-between-declarations-with-annotations)
for documentation.

**Active by default**: Yes - Since v1.22.0

### SpacingBetweenDeclarationsWithComments

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#blank-line-between-declaration-with-comments)
for documentation.

**Active by default**: Yes - Since v1.22.0

### SpacingBetweenFunctionNameAndOpeningParenthesis

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#spacing-between-function-name-and-opening-parenthesis) for
documentation.

**Active by default**: No

### StringTemplate

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#string-template) for documentation.

**Active by default**: Yes - Since v1.0.0

### TrailingCommaOnCallSite

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/) for documentation.

The default config comes from ktlint and follows these conventions:
- [Kotlin coding convention](https://kotlinlang.org/docs/coding-conventions.html#trailing-commas) recommends
trailing comma encourage the use of trailing commas at the declaration site and
leaves it at your discretion for the call site.
- [Android Kotlin style guide](https://developer.android.com/kotlin/style-guide) does not include
trailing comma usage yet.

**Active by default**: No

#### Configuration options:

* ``useTrailingCommaOnCallSite`` (default: ``true``) (android default: ``false``)

  Defines whether trailing commas are required (true) or forbidden (false) at call sites

### TrailingCommaOnDeclarationSite

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/) for documentation.

The default config comes from ktlint and follows these conventions:
- [Kotlin coding convention](https://kotlinlang.org/docs/coding-conventions.html#trailing-commas) recommends
trailing comma encourage the use of trailing commas at the declaration site and
leaves it at your discretion for the call site.
- [Android Kotlin style guide](https://developer.android.com/kotlin/style-guide) does not include
trailing comma usage yet.

**Active by default**: No

#### Configuration options:

* ``useTrailingCommaOnDeclarationSite`` (default: ``true``) (android default: ``false``)

  Defines whether trailing commas are required (true) or forbidden (false) at declaration sites

### TypeArgumentListSpacing

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#type-argument-list-spacing) for
documentation.

**Active by default**: No

### TypeParameterListSpacing

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#type-parameter-list-spacing) for
documentation.

**Active by default**: No

### UnnecessaryParenthesesBeforeTrailingLambda

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/experimental/#unnecessary-parenthesis-before-trailing-lambda)
for documentation.

**Active by default**: No

### Wrapping

See [ktlint docs](https://pinterest.github.io/ktlint/0.47.1/rules/standard/#wrapping) for documentation.

**Active by default**: Yes - Since v1.20.0

#### Configuration options:

* ``indentSize`` (default: ``4``)

  indentation size
