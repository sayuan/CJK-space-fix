# Introduction
According to the HTML specification, "An HTML user agent should treat end of
line in any of its variations as a word space in all contexts except
preformatted text".

This is okay in English, but we don't use spaces to separate words in
Chinese.  That unnecessary space make the sentence looks weird.  This
javascript file is aim to solve this problem.

# Usage
Just include the `cjk_space_fix.js` and invoke `cjkSpaceFix()`.

    <script type="text/javascript" src="path/to/cjk_space_fix.js"></script>
    <script type="text/javascript">
        window.onload = function () {
            cjkSpaceFix();
        }
    </script>

