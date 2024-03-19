 <!-- <link rel="stylesheet" href="/style.css"> -->

# Table of Contents
[Overview](#Overview)

[Quoting Code](#quoting-code)

[Fenced Code block](#fenced-code-block)

# Overview
Nearly all Markdown applications support the basic syntax outlined in the original Markdown design document. There are minor variations and discrepancies between Markdown processors — those are noted inline wherever possible. 

## Quoting Code

You can call out code or command within a sentence with single backticks. The text within the backticks will not be formatted. You can also press the `command + E` (Mac) or `Ctrl + E` (Windows/Linux) keyboard to insert a backticks for code block within a line of a Markdown.

Use `git status` to list all new or modified files that haven't been yet committed.

To format code or text into its own distinct block, use the triple backtracks

Some basic git commands are:
```
git status
git add
git commit
```
## Fenced Code block

You can create fenced code blocks by creating triple backticks ` ``` ` before and after the code block. You can place a blank line before and after code blocks to make the raw formatting easier to read.

```
function test (){
console.log("notice the blank line before this function)"
}

```

## Syntax Highlighting

You can add an optional language identifier to enable syntax highlighting in your fenced code block. Syntax highlighting changes the color and style of the source code to make it easier to read.

For example, to syntax highlight Ruby code

```ruby
require `redcarpet`
markdown=Redcarpet.new("Hello World!")
puts markdown.to_html
```
## Supported Color model
In issues, pull requests, and discussions, you can call out colors within a sentence using backticks. A supported color model within a backticks will display a visualization of the color.
The background color is `#ffffff` for light mode and `#000000` for light mode.
## Links

You can create an inline link by wrapping link text in brackets `[]` and then wrapping the URL in the parenthesis `()`.You can also use the keyboard shortcut `Command`+ `K` to create a link. When you have text selected, you can paste a URL from your clipboard to automatically create a link from the selection.

See an example link below: 

This page was created using Markdown in [<a href="https://github.com/GitHubMotiar/Learning_Markdown/wiki/Markdown-Basic-Syntax" class="no-underline"> **Git Hub Pages**</a>].

Now see below what was behind the output sentence above. For your understanding I have put the backend line in backticks. 

`This page was created using Markdown in [Git hub pages](https://github.com/GitHubMotiar/Learning_Markdown/wiki/Markdown-Basic-Syntax)`

## Lists

You can make an unordered list by preceding one or more lines of text with `-`, `*`, or `+`.
```
- George Washington
* John Adams
+ Mahatma Gandhi
```
- George Washington
* John Adams
+ Mahatma Gandhi

## Nested Lists

You can create a nested list by indenting one or more list items below another item.

```
1. First List item
   - Second list item
     - Third list item
```
1. First List item
   - Second list item
     - Third list item

For more examples, see the [GitHub Flavored Markdown Spec](https://github.github.com/gfm/#example-265).

## Task Lists

To create a task list, preface list item with a hyphen and spec followed by `[]`. To mark a task as complete, use `[x]`.

- [ ] Add delight to the experience when all tasks are complete :tada:
- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740

## Referencing issues and pull requests

You can bring up a list of suggested issues and pull requests within a repository by simply typing `#`. Type the issue or pull request number or title to filter the list, then press either tab or enter to complete the highlighted results. 
For more information, see [Autolinked references](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/autolinked-references-and-urls).

## Alerts

Alerts are a Markdown extension based on the blockquote syntax that you can use to emphasize critical information. On GitHub, they are displayed with distinctive colors and icons to indicate the significance of the content.
To add an alert, use a special blockquote line specifying the alert type, followed by the alert information in a standard blockquote. Five types of alerts are available:

> [!NOTE]
> Useful information that users should know, even when skimming content.
> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.

## Hide content from rendered output in Guthub
You can tell gitHub to hide content from rendered Markdown by placing the content in an HTML tag
<!-- This content will not appear in the rendered Markdown -->
