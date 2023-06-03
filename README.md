[Origin: Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

# Basic writing and formatting syntax

> Create sophisticated formatting for your prose and code on GitHub with simple syntax.


## Headings

To create a heading, add one to six `#` symbols before your heading text. The number of `#` you use will determine the hierarchy level and typeface size of the heading.

### A third-level heading

```markdown
# Basic writing and formatting syntax
## Headings
### A third-level heading
```

When you use two or more headings, GitHub automatically generates a table of contents that you can access by clicking <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-list-unordered" aria-label="The unordered list icon" role="img"><path d="M5.75 2.5h8.5a.75.75 0 0 1 0 1.5h-8.5a.75.75 0 0 1 0-1.5Zm0 5h8.5a.75.75 0 0 1 0 1.5h-8.5a.75.75 0 0 1 0-1.5Zm0 5h8.5a.75.75 0 0 1 0 1.5h-8.5a.75.75 0 0 1 0-1.5ZM2 14a1 1 0 1 1 0-2 1 1 0 0 1 0 2Zm1-6a1 1 0 1 1-2 0 1 1 0 0 1 2 0ZM2 4a1 1 0 1 1 0-2 1 1 0 0 1 0 2Z"></path></svg> within the file header.

… [Headings](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#headings)

![GitHub automatically generates a clickable table of contents based on multiple headings within a file, allowing users to easily navigate to different sections.](https://docs.github.com/assets/cb-82878/mw-1440/images/help/repository/headings-toc.webp)


## Styling text

You can indicate emphasis with bold, italic, strikethrough, subscript, or superscript text in comment fields and `.md` files.

| Style                  | Syntax             | Keyboard shortcut                                 | Example                                  | Output                                 |
|------------------------|--------------------|---------------------------------------------------|------------------------------------------|----------------------------------------|
| Bold                   | `** **` or `__ __` | `Command+B` (Mac) or `Ctrl+B` (Windows/Linux) | `**This is bold text**`                  | **This is bold text**                  |
| Italic                 | `* *` or `_ _`     | `Command+I` (Mac) or `Ctrl+I` (Windows/Linux) | `*This text is italicized*`              | *This text is italicized*              |
| Strikethrough          | `~~ ~~`            | None                                              | `~~This was mistaken text~~`             | ~~This was mistaken text~~             |
| Bold and nested italic | `** **` and `_ _`  | None                                              | `**This text is _extremely_ important**` | **This text is _extremely_ important** |
| All bold and italic    | `*** ***`          | None                                              | `***All this text is important***`       | ***All this text is important***       |
| Subscript              | `<sub> </sub>`     | None                                              | `<sub>This is a subscript text</sub>`    | <sub>This is a subscript text</sub>    |
| Superscript            | `<sup> </sup>`     | None                                              | `<sup>This is a superscript text</sup>`  | <sup>This is a superscript text</sup>  |

### Bold

**This is bold text**

```markdown
**This is bold text**
```

### Italicized

*This text is italicized*

```markdown
*This text is italicized*
```

### Striked

~~This was mistaken text~~

```markdown
~~This was mistaken text~~
```

### Extremely Important

**This text is _extremely_ important**

```markdown
**This text is _extremely_ important**
```

### All Important

***All this text is important***

```markdown
***All this text is important***
```

### Subscripted

<sub>This is a subscript text</sub>

```markdown
<sub>This is a subscript text</sub>
```

### Superscripted

<sup>This is a superscript text</sup>

```markdown
<sup>This is a superscript text</sup>
```


## Quoting text

You can quote text with a `>`.

Text that is not a quote  

> Text that is a quote  

```markdown
> Text that is a quote
```

In other words, adding two spaces at the end of each line in the cited text results in a line break.

> Text that is a quote  
> Text that is a quote

```markdown
> Text that is a quote  
> Text that is a quote  
```

```plain
🌵 Tip: When viewing a conversation, you can automatically quote text in a comment by highlighting the text, then typing R. You can quote an entire comment by clicking , then Quote reply. For more information about keyboard shortcuts, see "Keyboard shortcuts."
```

… [⌨ Keyboard shortcuts](https://docs.github.com/en/get-started/using-github/keyboard-shortcuts)  


## Quoting code

You can call out code or a command within a sentence with single backticks. The text within the backticks will not be formatted. You can also press the `Command+E` (Mac) or `Ctrl+E` (Windows/Linux) keyboard shortcut to insert the backticks for a code block within a line of Markdown.

Use `git status` to list all new or modified files that haven't yet been committed.

```markdown
Use `git status` to list all new or modified files that haven't yet been committed.
```

Some basic Git commands are:
```
git status
git add
git commit
```

````markdown
Some basic Git commands are:
```
git status
git add
git commit
```
````

For more information, see "[Creating and highlighting code blocks](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-and-highlighting-code-blocks)."

If you are frequently editing code snippets and tables, you may benefit from enabling a fixed-width font in all comment fields on GitHub. For more information, see "[About writing and formatting on GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/about-writing-and-formatting-on-github#enabling-fixed-width-fonts-in-the-editor)."


## 📍 Supported color models

In issues, pull requests, and discussions, you can call out colors within a sentence by using backticks. A supported color model within backticks will display a visualization of the color.

The background color is `#ffffff` for light mode and `#000000` for dark mode.

Here are the currently supported color models.

| Color | Syntax       | Example              | Output               |
|-------|--------------|----------------------|----------------------|
| HEX   | `#RRGGBB`    | `#0969DA`            | `#0969DA`            |
| RGB   | `rgb(R,G,B)` | `rgb(9, 105, 218)`   | `rgb(9, 105, 218)`   |
| HSL   | `hsl(H,S,L)` | `hsl(212, 92%, 45%)` | `hsl(212, 92%, 45%)` |

```plain
🌵 Notes:  

· A supported color model cannot have any leading or trailing spaces within the backticks.  
· The visualization of the color is only supported in issues, pull requests, and discussions.
```

… [Supported color models](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#supported-color-models)


## Links

You can create an inline link by wrapping link text in brackets `[ ]`, and then wrapping the URL in parentheses `( )`. You can also use the keyboard shortcut `Command+K` to create a link. When you have text selected, you can paste a URL from your clipboard to automatically create a link from the selection.

```markdown
[link text](URL)
```

You can also create a Markdown hyperlink by highlighting the text and using the keyboard shortcut `Command+V`. If you'd like to replace the text with the link, use the keyboard shortcut `Command+Shift+V`.

This site was built using [GitHub Pages](https://pages.github.com/).

```markdown
This site was built using [GitHub Pages](https://pages.github.com/).
```


```
🌵 Tip: GitHub automatically creates links when valid URLs are written in a comment. For more information, see "Autolinked references and URLs."
```

[Autolinked references and URLs](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/autolinked-references-and-urls)


## 📍 Section links

You can link directly to a section in a rendered file by hovering over the section heading to expose <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-link" aria-label="the link" role="img"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg>.

![By hovering over a section heading in a rendered file, you can link directly to that specific section.](https://docs.github.com/assets/cb-55935/mw-1440/images/help/repository/readme-links.webp)


## Relative links

You can define relative links and image paths in your rendered files to help readers navigate to other files in your repository.  

A relative link is a link that is relative to the current file. For example, if you have a README file in root of your repository, and you have another file in docs/CONTRIBUTING.md, the relative link to CONTRIBUTING.md in your README might look like this:

[Contribution guidelines for this project](docs/README.md)

```markdown
[Contribution guidelines for this project](docs/README.md)
```

GitHub will automatically transform your relative link or image path based on whatever branch you're currently on, so that the link or path always works. The path of the link will be relative to the current file. Links starting with `/` will be relative to the repository root. You can use all relative link operands, such as `./` and `../.`  

Relative links are easier for users who clone your repository. Absolute links may not work in clones of your repository - we recommend using relative links to refer to other files within your repository.  


## 🔫 Images

[Images](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#images)

![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://myoctocat.com/assets/images/base-octocat.svg)

GitHub supports embedding images into your issues, pull requests, discussions, comments and .md files. You can display an image from your repository, add a link to an online image, or upload an image. For more information, see "[Uploading assets](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#uploading-assets)."


Here are some examples for using relative links to display an image.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/25423296/163456776-7f95b81a-f1ed-45f7-b7ab-8fa810d529fa.png">
  <source media="(prefers-color-scheme: light)" srcset="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
  <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
</picture>

## Lists

- George Washington
* John Adams
+ Thomas Jefferson

1. James Madison
2. James Monroe
3. John Quincy Adams


### Nested Lists

1. First list item
    1. First nested list item
        1. Second nested list item


- First list item
  - First nested list item
    - Second nested list item

1. First list item
    - First nested list item
        - Second nested list item

## Task lists

- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:

- [ ] \(Optional) Open a followup issue


## Mentioning people and teams

@github/support What do you think about these updates?


## Referencing issues and pull requests

For more information, see "[Autolinked references and URLs.](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/autolinked-references-and-urls)"


## Referencing external resources

For more information, see "[Configuring autolinks to reference external resources.](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/configuring-autolinks-to-reference-external-resources)"


## Uploading assets

You can upload assets like images by dragging and dropping, selecting from a file browser, or pasting. You can upload assets to issues, pull requests, comments, and .md files in your repository.

## Using emoji

@octocat :+1: This PR looks great - it's ready to merge! :shipit:

For a full list of available emoji and codes, see [the Emoji-Cheat-Sheet](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md).


## Paragraphs

You can create a new paragraph by leaving a blank line between lines of text.


## Footnotes

Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

[^1]: My reference.
[^2]: To add line breaks within a footnote, prefix new lines with 2 spaces.
  This is a second line.


## Hiding content with comments

<!-- This content will not appear in the rendered Markdown -->


## Ignoring Markdown formatting

Let's rename \*our-new-project\* to \*our-old-project\*.


## Disabling Markdown rendering

When viewing a Markdown file, you can click  at the top of the file to disable Markdown rendering and view the file's source instead.

![](https://docs.github.com/assets/cb-24194/mw-1440/images/help/writing/display-markdown-as-source.webp)

<!-- Disabling Markdown rendering enables you to use source view features, such as line linking, which is not possible when viewing rendered Markdown files. -->

… [Disabling Markdown rendering](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#disabling-markdown-rendering)


## Further reading

- [GitHub Flavored Markdown Spec](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/about-writing-and-formatting-on-github)
- "[About writing and formatting on GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/about-writing-and-formatting-on-github)"
- "[Working with advanced formatting](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting)"
- "[Quickstart for writing on GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github)"
