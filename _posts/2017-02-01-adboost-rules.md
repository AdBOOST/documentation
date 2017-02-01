---
layout: default
title:  "AdBOOST Rules"
date:   2017-02-01 09:08:30 -0600
category: adboost_core
tags: [adboost, rules]
---

## AdBOOST Rules

* TOC
{:toc}

### Introduction

Rule system is an inseparable and core part of AdBOOST, which you will encouter many times during his usage. This page explains what is the reason of our inclination to rules, where you can find them and most important, how to use them and get the most out of them.

### Where to find the rules

Here is the comprehensive list of all rules locations:

1. Feed filter rules
2. Feed editor rules
3. Product Group assign rules
4. Keyword Pattern filter rules
5. Ad Pattern filter rules
6. Export filter rules
7. Export CPC edit rules
8. Notifications setup

### Rule types

There are two types of rules:

1. Filter rules - can be found as a single container and consist of predicates and conditions
2. Modifier rules - can be found as a set of orderable containers that consist of filter predicates and modifier actions

Example 1: Filter rule with two predicates, first with two conditions, second with one condition

{% include image_tag.html url="/AdBOOST/images/rules/FilterRule.png" alt="Filter Rule" style="" %}

Example 2: Two modifier rules. First with one predicate, two conditions and one actions, second with no predicates and two actions.

{% include image_tag.html url="/AdBOOST/images/rules/ModifierRules.png" alt="Modifier Rules" style="" %}

- **If you leave predicate part of any rule empty, it will match all items**.
- Modifier rules, same as rule actions are orderable - Drag&Drop by <i class="glyphicon glyphicon-resize-vertical">&nbsp;</i>handle.
- **Rules are applied sequentially and order matters**. If you modify some of item properties in one rule, all following rules will show only informative number of covered items but correct result of all previous rule actions applied in sequential order. See the screen below.

{% include image_tag.html url="/AdBOOST/images/rules/RulesVariableRewrite.png" alt="Rules Variable Rewrite" style="" %}

### Rule structure

#### Predicates

Every rule predicate has following structure:

OPERAND - OPERATOR - VALUE

- OPERAND - feed property, that can either exist in feed or have been created as a virtual property in Feed Schema Settings. These properties can be numeric - properties in numeric1, numeric2 or other_numeric categories, or non-numeric - every other feed property

{% include image_tag.html url="/AdBOOST/images/rules/RuleOperand.png" alt="Rule Operand" style="" %}

- OPERATOR - set of operations that differ for numeric and non-numeric feed properties (See the screen below)

{% include image_tag.html url="/AdBOOST/images/rules/RuleOperators.png" alt="Rule Operators" style="" %}

