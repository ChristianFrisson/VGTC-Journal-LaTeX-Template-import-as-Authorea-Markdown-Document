Bibliography Instructions
=========================

-   Sort all bibliographic entries alphabetically but the last name of
    the first author. This LaTeX/bibTeX template takes care of this
    sorting automatically.

-   Merge multiple references into one; e.g., use \cite{Max:1995:OMF,Kitware:2003}
    (not \cite{Kitware:2003}\cite{Max:1995:OMF}). Within each set of
    multiple references, the references should be sorted in ascending
    order. This LaTeX/bibTeX template takes care of both the merging and
    the sorting automatically.

-   Verify all data obtained from digital libraries, even ACM’s DL and
    IEEE Xplore etc. are sometimes wrong or incomplete.

-   Do not trust bibliographic data from other services such as
    Mendeley.com, Google Scholar, or similar; these are even more likely
    to be incorrect or incomplete.

-   Articles in journal—items to include:

    -   author names

    -   title

    -   journal name

    -   year

    -   volume

    -   number

    -   month of publication as variable name (i.e., {jan} for January,
        etc.; month ranges using {jan \#{/}\# feb} or {jan \#{--}\#
        feb})

-   use journal names in proper style: correct: “IEEE Transactions on
    Visualization and Computer Graphics”, incorrect: “Visualization and
    Computer Graphics, IEEE Transactions on”

-   Papers in proceedings—items to include:

    -   author names

    -   title

    -   abbreviated proceedings name: e.g., “Proc.\\ CONF\_ACRONYNM”
        without the year; example: “Proc.\\ CHI”, “Proc.\\ 3DUI”,
        “Proc.\\ Eurographics”, “Proc.\\ EuroVis”

    -   year

    -   publisher

    -   town with country of publisher (the town can be abbreviated for
        well-known towns such as New York or Berlin)

-   article/paper title convention: refrain from using curly brackets,
    except for acronyms/proper names/words following dashes/question
    marks etc.; example:

    -   paper “Marching Cubes: A High Resolution 3D Surface Construction
        Algorithm”

    -   should be entered as “{M}arching {C}ubes: A High Resolution {3D}
        Surface Construction Algorithm” or “{M}arching {C}ubes: A high
        resolution {3D} surface construction algorithm”

    -   will be typeset as “Marching Cubes: A high resolution 3D surface
        construction algorithm”

-   for all entries

    -   DOI can be entered in the DOI field as plain DOI number or as
        DOI url; alternative: a url in the URL field

    -   provide full page ranges AA--BB

-   when citing references, do not use the reference as a sentence
    object; e.g., wrong: “In \cite{Lorensen:1987:MCA} the authors describe …”,
    correct: “Lorensen and Cline \cite{Lorensen:1987:MCA} describe …”