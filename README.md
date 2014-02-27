<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#sec-1">1. What's this?</a></li>
<li><a href="#sec-2">2. Function</a></li>
<li><a href="#sec-3">3. Sample</a></li>
<li><a href="#sec-4">4. Install</a>
<ul>
<li><a href="#sec-4-1">4.1. If use package.el</a></li>
<li><a href="#sec-4-2">4.2. If use el-get.el</a></li>
<li><a href="#sec-4-3">4.3. If use auto-install.el</a></li>
<li><a href="#sec-4-4">4.4. Manually</a></li>
<li><a href="#sec-4-5">4.5. Dependency</a></li>
</ul>
</li>
<li><a href="#sec-5">5. Tested On</a></li>
</ul>
</div>
</div>

# What's this?

This is a extension of Emacs that provide the functions of auto-complete for handling Programmable Completion.  
You can define the source of auto-complete.el to handle pcomplete.

# Function

-   ac-pcmp/get-ac-candidates
-   ac-pcmp/do-ac-action
-   ac-pcmp/self-insert-command-with-ac-start

# Sample

```lisp
(defvar ac-source-xxxx
  '((candidates . ac-pcmp/get-ac-candidates)
    (prefix . "xxxx \\(.*\\)")
    (symbol . "x")
    (requires . 0)
    (cache)
    (action . ac-pcmp/do-ac-action)))
```

# Install

## If use package.el

2014/02/27 It's available by using melpa.

## If use el-get.el

2014/02/26 Now application

## If use auto-install.el

```lisp
(auto-install-from-url "https://raw.github.com/aki2o/auto-complete-pcmp/master/auto-complete-pcmp.el")
```

-   In this case, you need to install each of the following dependency.

## Manually

Download bbdb-.el and put it on your load-path.

-   In this case, you need to install each of the following dependency.

## Dependency

-   [auto-complete.el](https://github.com/auto-complete/auto-complete)
-   [log4e.el](https://github.com/aki2o/log4e)
-   [yaxception.el](https://github.com/aki2o/yaxception)

# Tested On

-   Emacs &#x2026; GNU Emacs 24.3.1 (i686-pc-linux-gnu, GTK+ Version 3.4.2) of 2013-08-22 on chindi02, modified by Debian
-   auto-complete.el &#x2026; 1.4.0
-   log4e.el &#x2026; 0.2.0
-   yaxception.el &#x2026; 0.1


**Enjoy!!!**

