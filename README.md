<image src="logo.png" width="300px">
</image>

# VisionMark

Highly extended specification for Markdown, intended for complex documents.

`VisionMark` is an attempt to solve the problem of **incompatibility of different Markdown implementations**, while pushing the capabilities of `CommonMark` to the limits.

## The era of plain-text formatting

VisionMark can produce highly complex documents, while being intuitive for the user. Here is an example of what it can do:

```
== Header <id> // Comment

Lorem ipsum *dolor* sit _amet_. The link to header is @id.

`code` is no more a stack of "`". Now you can do like this:

`
int code = 0;
code.parse();
`

or something like this:

+
int code = 0;
code.parse();
+

Do you like footnotes? +fn(1)

+fn(1):  Yes, I do!

Tables are easy-to-create, no more spawning dashes!

+table(3x3)
column header; **bold formatted** header; Table can now be created within one line!;
+fm(2x+3 \int); ; <- see this empty cell?;
+br +br +br; <- these are breaks; the end.
+

As you've seen, new _objects_ start with a plus sign, then you specify the type of an object and its arguments. That's it!

> How do you make an image?
> +img(path/to/image, with a caption like this)

There are more advanced examples:

- List of some items
--x New Task list item
--x Second item!
--0 Incomplete task

^ Right there you have seen that we do not need an indention to make a secondary list.

> Like this you can specify a collapsible list summary
_ And here you start a one-line explanation.
_ But it can also span multiple paragraphs!

The goal of such `markup` is to move further away from HTML-tags.
```

## How to use?

Documentation addressing various syntax is provided within Wiki section.

## Further exploration

Since VisionMark is just a concept, you are free to modify or use it as a base for text editors and renderers and other types of software. VisionMark is being distributed under `MIT License`.
