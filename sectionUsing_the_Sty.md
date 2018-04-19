Using the Style Template
========================

-   If you receive compilation errors along the lines of
    “`Package ifpdf Error: Name clash, \ifpdf is already defined`” then
    please add a new line “`\let\ifpdf\relax`” right after the
    “`\documentclass[journal]{vgtc}`” call. Note that your error is due
    to packages you use that define “`\ifpdf`” which is obsolete (the
    result is that `\ifpdf` is defined twice); these packages should be
    changed to use ifpdf package instead.

-   Note that each author’s affiliations have to be provided in the
    author footer on the bottom-left corner of the first page. It is
    permitted to merge two or more people from the same institution as
    long as they are shown in the same order as in the overall author
    sequence on the top of the first page. For example, if authors A, B,
    C, and D are from institutions 1, 2, 1, and 2, respectively, then it
    is ok to use 2 bullets as follows:

    -   A and C are with Institution 1. E-mail: {a$|$c}@i1.com.

    -   B and D are with Institution 2. E-mail: {b$|$d}@i2.org.

-   The style uses the hyperref package, thus turns references into
    internal links. We thus recommend to make use of the
    “`\autoref{reference}`” call (instead of “`Figure~\ref{reference}`”
    or similar) since “`\autoref{reference}`” turns the entire reference
    into an internal link, not just the number. Examples: and .

-   The style automatically looks for image files with the correct
    extension (eps for regular LaTeX; pdf, png, and jpg for pdfLaTeX),
    in a set of given subfolders (figures/, pictures/, images/). It is
    thus sufficient to use “`\includegraphics{CypressView}`” (instead of
    “`\includegraphics{pictures/CypressView.jpg}`”).

-   For adding hyperlinks and DOIs to the list of references, you can
    use “`\bibliographystyle{abbrv-doi-hyperref-narrow}`” (instead of
    “`\bibliographystyle{abbrv}`”). It uses the doi and url fields in a
    bibTeX entry and turns the entire reference into a link, giving
    priority to the doi. The doi can be entered with or without the
    “`http://dx.doi.org/`” url part. See the examples in the bibTeX file
    and the bibliography at the end of this template.\
    **Note 1:** occasionally (for some LaTeX distributions) this
    hyper-linked bibTeX style may lead to **compilation errors**
    (“`pdfendlink ended up in different nesting level ...`”) if a
    reference entry is broken across two pages (due to a bug in
    hyperref). In this case make sure you have the latest version of the
    hyperref package (i.e., update your LaTeX installation/packages) or,
    alternatively, revert back to
    “`\bibliographystyle{abbrv-doi-narrow}`” (at the expense of removing
    hyperlinks from the bibliography) and try
    “`\bibliographystyle{abbrv-doi-hyperref-narrow}`” again after some
    more editing.\
    **Note 2:** the “`-narrow`” versions of the bibliography style use
    the font “PTSansNarrow-TLF” for typesetting the DOIs in a compact
    way. This font needs to be available on your LaTeX system. It is
    part of the [“paratype” package](https://www.ctan.org/pkg/paratype),
    and many distributions (such as MikTeX) have it automatically
    installed. If you do not have this package yet and want to use a
    “`-narrow`” bibliography style then use your LaTeX system’s package
    installer to add it. If this is not possible you can also revert to
    the respective bibliography styles without the “`-narrow`” in the
    file name.\
    DVI-based processes to compile the template apparently cannot handle
    the different font so, by default, the template file uses the
    `abbrv-doi` bibliography style but the compiled PDF shows you the
    effect of the `abbrv-doi-hyperref-narrow` style.