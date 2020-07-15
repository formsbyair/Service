---
title: Boolean/Option Tag Values
type: platform
---

Tags for **True/False** and **Option** type questions are evaluated as follows:

|Tag|Result In Form|Result Everywhere Else|
|---|---|---|
|&lt;&lt;MyTrueFalseQuestion&gt;&gt;|true or false|Yes or No|
|&lt;&lt;MyOption&gt;&gt;|true or false|Question Title or &lt;blank&gt;|

The intent is to display a user-friendly value by default, however this can lead to confusion when you want to sue these tags in expressions.

To make it more explicit, you can now use the **Value** tag property to refer to the underlying value for true/false or option questions.

|Expression Using Value Property outside of a form|Equivalent To|
|---|---|
|&apos;&lt;&lt;MyTrueFalseQuestion.Value&gt;&gt;&apos; == &apos;true&apos;|&apos;&lt;&lt;MyTrueFalseQuestion&gt;&gt;&apos; == &apos;Yes&apos;|
|&apos;&lt;&lt;MyOption.Value&gt;&gt;&apos; == &apos;true&apos;|&apos;&lt;&lt;MyOption&gt;&gt;&apos; != &apos;&apos;|