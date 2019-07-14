# ift-highlighter

Highlighter for ift file(interactive fiction text).

## Usage

Ift is a kind of file based on XML, its a part of [if-maker](https://github.com/DiscreteTom/if-maker).

This extension provide code snippets and syntax highlighting for ift file.

## ift file format

Though ift is based on XML, you don't have to write `<?xml version="1.0"?>` and root element, if-maker will add it for you.

```xml
#include otherIftFile

<story name="story-id">
	story text here
	<if condition="python code here">
		conditional story text here
	</if>
	<while condition="python code here">
		repeat story text here
	</while>
	{{ value reference here }}
	<code>python code here</code>
	<input>variable-name</input>
</story>
```

`#include` field can include other ift files in current file. Ift file name can not contain spaces. `#include` must be the top a ift file. After `#include` there must be an empty line.