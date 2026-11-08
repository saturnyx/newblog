+++
title = "A Blog in Zola"
date = 2025-08-16
description = ""
+++

# Why Zola

Last month, I came across this cool project called [Zola](https://getzola.org). For a long time I have been wanting to replace my static site generator for my original [blog](https://oldblog.saturnyx.dev/), which used [Jekyll](https://jekyllrb.com/). As much I love Ruby as a language, Jekyll's complex dependencies and single-threaded compilation made it hard to use. So, I switched to Zola. It seems a like a pretty new project but I know it will get mature soon.

# A few issues I ran into

So, the transition was not the most seamless. Zola lacked a lot of the features that Jekyll had. For example, Zola has,

- No plugin ecosystem,
- No Github actions native support
- No large theme ecosystem

But these, were no big issues for my simple blog, I loved my own theme and I did not need complex plugins.

# Things to love Zola for

Zola makes up for its lack of a plugin ecosystem by bundling a lot of features into its single binary.

## Sassy Style Sheets

Yes. SASS is natively supported by Zola, and it makes my life so much easier. Though modern CSS is already similar to SASS to some extent, having native SASS compilation is much more simpler than having to use it has a plugin.

## Built-in ToC and Search Index

This is something that I haven't really utilized in my blog yet, but I am likely to add it in the near future. Zola extracts and builds a search index, at build time, which can then be paired with a small JS library (like MiniSearch or Elasticlunr.js).

## Syntax Highlighting

Build-time syntax highlighting is also one of the key features of Zola. It uses TextMate grammars (the same engine as VS Code), which tend to produce more accurate highlighting for modern languages than the older Pygments-style lexers.

# Conclusion

All in all, I have no regrets on my transition to Zola and am currently waiting on new updates.
