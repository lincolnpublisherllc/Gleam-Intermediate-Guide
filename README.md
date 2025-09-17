Gleam Intermediate Guide — Code Extraction

This archive contains all detected code snippets from Gleam Intermediate Guide.docx, grouped by chapter.

What's inside
/
├─ 00_Unknown/            # Snippets that appear before the first chapter heading
├─ 01_Chapter_1/
├─ 02_Chapter_2/
├─ …
├─ 14_Chapter_14/
├─ manifest.csv           # Index of every snippet (chapter, file name, start paragraph, lines, ext)
└─ README.txt


Each chapter folder contains files named:

snippet_01.gleam
snippet_02.erl
snippet_03.sh
snippet_04.json
snippet_05.txt
...


File extensions are inferred from content:

.gleam for Gleam code

.erl for Erlang

.sh for CLI commands

.json for JSON-like blocks

.txt when the type is unclear

Quick start

Unzip the archive.

Open manifest.csv in Excel or any CSV viewer.

Filter by chapter or ext to find code you need.

Review start_paragraph_index if you want to jump back to the source DOCX.

How snippets were detected

A snippet is a contiguous block of paragraphs that look like code. The detector looks for:

Indentation at the start of a line

Common code symbols such as (, ), {, }, ->, :

Gleam/Erlang keywords (for example pub fn, type, List., Dict., dbg:)

CLI command lines starting with common tools (gleam, git, erl, sudo, brew, choco, cd, mkdir, rm, ls, curl)

Fenced blocks or comment-style markers

Chapters are identified by headings like Chapter 1, Chapter 2, and so on. Content found before the first heading is placed in 00_Unknown.

Counts (for a quick check)

00_Unknown: 7 snippets

01_Chapter_1: 28

02_Chapter_2: 27

03_Chapter_3: 31

04_Chapter_4: 31

05_Chapter_5: 25

06_Chapter_6: 33

07_Chapter_7: 28

08_Chapter_8: 40

09_Chapter_9: 15

10_Chapter_10: 20

11_Chapter_11: 23

12_Chapter_12: 17

13_Chapter_13: 31

14_Chapter_14: 16

Tips for review

Search inside chapter folders for function names, modules, or commands.

Use the CSV to spot unusually long or short snippets and verify them first.

If a snippet looks like mixed content, check neighboring files in the same chapter.

Reclassify extensions if needed; filenames are neutral on purpose.

Known limitations

Some prose lines that include many symbols may be classified as code.

Mixed language blocks may be stored as .txt or .sh.

If a chapter heading in the DOCX uses a nonstandard format, that content may fall into 00_Unknown.

How to request refinements

Tell me any of the following and I’ll regenerate:

A list of keywords or patterns to treat as code or to ignore

A stricter split between CLI vs. source files

Custom filenames (for example http_client.gleam instead of snippet_03.gleam)

Merging very short snippets into the previous one

Files

Archive: gleam_code_extract.zip

Index: manifest.csv

This README: README.txt

Download the ZIP if you need it again:
gleam_code_extract.zip
