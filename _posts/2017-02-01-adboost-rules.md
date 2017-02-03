---
layout: default
title:  "AdBOOST Rules"
date:   2017-02-01 09:08:30 -0600
category: adboost_core
tags: [adboost, rules]
---

# AdBOOST Rules
<br/>

* TOC
{:toc}

## Introduction

Rule system is an inseparable and core part of AdBOOST, which you will encouter many times during his usage. From the moment, when your items enter the AdBOOST for a first time (as a part of the data feed during its first processing) until they leave it towards target advertising network, they are filtered and modified multiple times. To ensure that you can segment your items and modify them to fit your needs, we use rules. In later parts of this guide, you will find out, where you can find the rules and most important, how to use them and get the most out of them.

## Where to find the rules

Here is the comprehensive list of all rules locations:

1. Feed filter rules
2. Feed editor rules
3. Product Group assign rules
4. Keyword Pattern filter rules
5. Ad Pattern filter rules
6. Export filter rules
7. Export CPC edit rules
8. Notifications setup

## Rule types

There are two types of rules:

1. **Filter rules** - can be found as a single container and consist of predicates and conditions
2. **Modifier rules** - can be found as a set of orderable containers that consist of filter predicates and modifier actions

**Example 1**: Filter rule with two predicates, first with two conditions, second with one condition

{% include image_tag.html url="/images/rules/FilterRule.png" alt="Filter Rule" style="" %}

**Example 2**: Two modifier rules. First with one predicate, two conditions and one actions, second with no predicates and two actions.

{% include image_tag.html url="/images/rules/ModifierRules.png" alt="Modifier Rules" style="" %}

- **If you leave predicate part of any rule empty, it will match all items**
- Modifier rules, same as rule actions are orderable - Drag&Drop by <i class="glyphicon glyphicon-resize-vertical">&nbsp;</i>handle
- **Rules are applied sequentially and order matters**. If you modify some of item properties in one rule, all following rules will show only informative number of covered items but correct result of all previous rule actions applied in sequential order. See the screen below

{% include image_tag.html url="/images/rules/RulesVariableRewrite.png" alt="Rules Variable Rewrite" style="" %}

## Rule structure

This section describes individual parts of every rule, starting at top-level and increasing granularity.

### Predicates

Every rule predicate is a collection of conditions with following structure:

OPERAND - OPERATOR - VALUE

Predicates, same as conditions can be combined by logical operators AND (all conditions are met) and OR (at least one condition is met).

- **OPERAND** - feed property, that can either exist in feed or have been created as a virtual property in Feed Schema Settings. These properties can be **numeric** - properties in numeric1, numeric2 or other_numeric categories, or **generic** - every other feed property

{% include image_tag.html url="/images/rules/RuleOperand.png" alt="Rule Operand" style="" %}

- **OPERATOR** - set of operations that differ for numeric and generic feed properties

{% include image_tag.html url="/images/rules/RuleOperators.png" alt="Rule Operators" style="" %}

- **VALUE** - **case-insensitive** text value that differs with operator because there are three types of them:

    - **Operator without value** - Not empty

    - **Basic operators** - =, !=, >, <, >=, <=, Starts with, Ends with, Contains, Does not contain, Regex

    {% include image_tag.html url="/images/rules/BasicOperator.png" alt="Basic Operator" style="" %}

    - **Batch operators** - Contains any, Does not contain any

    {% include image_tag.html url="/images/rules/BatchOperator.png" alt="Batch Operator" style="" %}

### Actions

Actions can be found only in modifier rules because they change values of properties for items that fit the conditions of one specific modifier rule.

Structure of actions is very simmilar to the one of predicates:

OPERAND - OPERATOR - VALUE/PARAMETERS

- **OPERAND** - feed property, that can either exist in feed or have been created as a virtual property in Feed Schema Settings.

- **OPERATOR** - set of operations summorted by AdBOOST

{% include image_tag.html url="/images/rules/RuleActions.png" alt="Rule Actions" style="" %}

- **VALUE/PARAMS** - this property differs for every operator:

    - **Replace** - find one string and replace it with another

    {% include image_tag.html url="/images/rules/ActionReplace.png" alt="Replace Action" style="" %}

    - **Set** - replace property value with static content or with value of other property

    {% include image_tag.html url="/images/rules/ActionSet.png" alt="Set Action" style="" %}

    - **Cut** - find string in value and remove everything on its left/right including/without itself

    {% include image_tag.html url="/images/rules/ActionRCut.png" alt="Cut Action" style="" %}

    - **Regex** - same as replace but instead of string to find, you should provide regular expression

    {% include image_tag.html url="/images/rules/ActionRegex.png" alt="Regex Action" style="" %}

    - **Capitalization** - set capitalization policy

    {% include image_tag.html url="/images/rules/ActionCapitalization.png" alt="Capitalization Action" style="" %}

    - **Uppercase** - make all letters in property value uppercase

    {% include image_tag.html url="/images/rules/ActionUppercase.png" alt="Uppercase Action" style="" %}

    - **Round** - if the selected property is numeric, round it's value to fixed decimal places (usefull after math operations)

    {% include image_tag.html url="/images/rules/ActionRound.png" alt="Round Action" style="" %}

    - **Math expression** - take one property, apply math operation to it and save it as a value of another property

    {% include image_tag.html url="/images/rules/ActionMathExpression.png" alt="MathExpression Action" style="" %}

    - **Batch remove** - remove all listed strings from value

    {% include image_tag.html url="/images/rules/ActionBatchRemove.png" alt="BatchRemove Action" style="" %}

    - **Remove colors** - remove color names in selected language

    {% include image_tag.html url="/images/rules/ActionRemoveColors.png" alt="RemoveColors Action" style="" %}

    - **Strip HTML** - remove any HTML tags (ussualy enclosed in <> tags)

    {% include image_tag.html url="/images/rules/ActionStripHtml.png" alt="StripHtml Action" style="" %}

    - **Hash** - create unique hash from one property value and save it as a value of another property

    {% include image_tag.html url="/images/rules/ActionHash.png" alt="Hash Action" style="" %}



