---
layout: post
title:  "Ruby's Forwardable"
date:   2021-12-08 21:37:12 +0700
categories: code ruby oop
---

### What does Ruby's forwardable library do?
Sometimes you find that you are using one method to call another object's variable<br />
*For example: User#first_name refers to Account#first_name*

Forwardable can help with de-duplicating your code.
By adding
`require 'forwardable'` and
`def_delegators :account, :first_name`
we can access user.first_name.



