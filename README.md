# ift-highlighter

Highlighter for IFT file(interactive fiction text).

## Usage

IFT is a kind of file based on XML, its a part of [if-maker](https://github.com/DiscreteTom/if-maker).

This extension provide code snippets and syntax highlighting for IFT file.

## IFT file format

Though IFT is based on XML, you don't have to write `<?xml version="1.0"?>` and root element, if-maker will add it for you.

```xml
#include file1.ift file2.ift

<story id="story-id">
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

`#include` field can include other IFT files in current file. IFT file name can not contain spaces.