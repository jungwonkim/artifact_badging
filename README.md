# acm_badging
This guide shows you how to include the ACM or NISO Artifact badges in your ACM or IEEE paper.

## Get the sample LaTeX code and vector images of the artifact badges.
    $ git clone https://github.com/jungwonkim/artifact_badging.git

### Step 1. Include the TikZ and Background packages.
    \usepackage{tikz}
    \usepackage[pages=some]{background}

### ACM: Step 2. Copy the following LaTeX code at right after \maketitle in your main LaTeX source file.
    \maketitle

    \backgroundsetup{opacity=1, scale=1, angle=0, contents={
    \begin{tikzpicture}[remember picture, overlay]
    \node[anchor=north east, inner xsep=50pt, inner ysep=10pt] at (current page.north east) {
    \href{https://www.acm.org/publications/policies/artifact-review-and-badging-current}{
    \includegraphics[width=50pt]{artifacts_evaluated_functional_v1.1.pdf}
    \includegraphics[width=50pt]{artifacts_evaluated_reusable_v1.1.pdf}
    \includegraphics[width=50pt]{artifacts_available_v1.1.pdf}
    \includegraphics[width=50pt]{results_reproduced_v1.1.pdf}
    \includegraphics[width=50pt]{results_replicated_v1.1.pdf}
    }};
    \end{tikzpicture}
    }}
    \BgThispage

### ACM: Step 3. Make comments in \includegraphcs not for your badges. If your paper has Available and Reproduced badges. Your LaTeX code looks like:
    \maketitle

    \backgroundsetup{opacity=1, scale=1, angle=0, contents={
    \begin{tikzpicture}[remember picture, overlay]
    \node[anchor=north east, inner xsep=50pt, inner ysep=10pt] at (current page.north east) {
    \href{https://www.acm.org/publications/policies/artifact-review-and-badging-current}{
    %\includegraphics[width=50pt]{artifacts_evaluated_functional_v1.1.pdf}
    %\includegraphics[width=50pt]{artifacts_evaluated_reusable_v1.1.pdf}
    \includegraphics[width=50pt]{artifacts_available_v1.1.pdf}
    \includegraphics[width=50pt]{results_reproduced_v1.1.pdf}
    %\includegraphics[width=50pt]{results_replicated_v1.1.pdf}
    }};
    \end{tikzpicture}
    }}
    \BgThispage

### IEEE: Step 2. Copy the following LaTeX code at right after \maketitle in your main LaTeX source file.
    \maketitle

    \backgroundsetup{opacity=1, scale=1, angle=0, contents={
    \begin{tikzpicture}[remember picture, overlay]
    \node[anchor=north east, inner xsep=50pt, inner ysep=5pt] at (current page.north east) {
    \href{https://doi.org/10.3789/niso-rp-31-2021}{
    \includegraphics[width=40pt]{Research_Objects.png}
    \includegraphics[width=40pt]{Open_Research.png}
    \includegraphics[width=40pt]{Results_Reproduced.png}
    \includegraphics[width=40pt]{Findings_Replicated.png}
    }};
    \end{tikzpicture}
    }}
    \BgThispage

### IEEE: Step 3. Make comments in \includegraphcs not for your badges. If your paper has ROR and RR badges. Your LaTeX code looks like:
    \maketitle

    \backgroundsetup{opacity=1, scale=1, angle=0, contents={
    \begin{tikzpicture}[remember picture, overlay]
    \node[anchor=north east, inner xsep=50pt, inner ysep=5pt] at (current page.north east) {
    \href{https://doi.org/10.3789/niso-rp-31-2021}{
    \includegraphics[width=40pt]{Research_Objects.png}
    %\includegraphics[width=40pt]{Open_Research.png}
    \includegraphics[width=40pt]{Results_Reproduced.png}
    %\includegraphics[width=40pt]{Findings_Replicated.png}
    }};
    \end{tikzpicture}
    }}
    \BgThispage
    
### Done.
