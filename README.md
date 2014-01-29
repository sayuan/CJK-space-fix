# Introduction

According to the HTML specification, "An HTML user agent should treat end of
line in any of its variations as a word space in all contexts except
preformatted text".

This is okay in English, but we don't use spaces to separate words in
Chinese.  That unnecessary space make the sentence looks weird.  This
javascript file is aim to solve this problem.

根據 HTML 規格書: "所有的換行字元都應該被視為空白，
只有 preformatted text 是例外"。

這在英文中是沒有問題的，但是在中文，我們並不使用空白來分隔字詞。
這些多餘的空白會使得句子看起來很奇怪，而這支 javascript 程式就是用來解決此問題。

# Example

HTML source:

    <p>
    這是一句很長的話
    中間有換行。
    </p>

What the browser show:

    這是一句很長的話 中間有換行。

What we actually want:

    這是一句很長的話中間有換行。

# Usage
Just include the `cjk_space_fix.js` and invoke `cjkSpaceFix()`.

    <script type="text/javascript" src="path/to/cjk_space_fix.js"></script>
    <script type="text/javascript">
        window.onload = function () {
            cjkSpaceFix();
        };
    </script>

