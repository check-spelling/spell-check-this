<!-- See https://github.com/check-spelling/check-spelling/wiki/Configuration-Examples%3A-advice --> <!-- markdownlint-disable MD033 MD041 -->
<details><summary>If you see a bunch of garbage and it relates to a binary-ish string</summary>

Please add a file path to the `excludes.txt` file instead of just accepting the garbage.

File paths are Perl 5 Regular Expressions - you can [test](
https://www.regexplanet.com/advanced/perl/) yours before committing to verify it will match your files.

`^` refers to the file's path from the root of the repository, so `^README\.md$` would exclude [README.md](
../tree/HEAD/README.md) (on whichever branch you're using).
</details>
