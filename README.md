# The Geometry of Scope: Context, Visibility, and Translation Across Formal Systems

Flyxion, Independent Researcher. October 2026.

This repository holds the LaTeX source of a mathematical essay on how formal languages, operating systems, computational environments, and interactive virtual worlds organize context, visibility, and permissible operations. The compiled essay is available as a PDF at [The Geometry of Scope](https://standardgalactic.github.io/computation/geometry-of-scope.pdf).

## The framework

Despite their differences, many such systems admit representations in terms of nested or overlapping domains, locally available information, transition relations, and structure-preserving mappings. The essay develops a framework for comparing them without presupposing that they are equivalent. Its primitive construction is a contextual representation system: a small category of contexts, a set of underlying states, a presheaf of context-indexed observations coherent with the restriction arrows, an assignment of admissible actions, and a partial transition function.

Within this framework, knowledge, presentation, and authority are independent assignments, so hierarchical containment alone forces no monotonicity of visibility or permission. Navigation between contexts is separated from disclosure within a context by an explicit commutation criterion. Filesystems, shell environments, lexical scope, access control, and game worlds are treated as instances, and the orientation of information flow is identified as the structural feature that distinguishes sections over regions from environments built by accumulation.

## Results

For every system the essay constructs a canonical presheaf of observational distinctions and characterizes it by a universal property. It characterizes in the same way the coarsest quotient of the state space compatible with a chosen family of contexts, and it identifies the terminal system observed through a fixed observation presheaf with its global sections. Failures of local-to-global reconstruction are classified and exhibited by finite examples.

Translations between systems are analyzed by what they preserve, reflect, collapse, or invent. Observational distinctions are preserved by every translation and reflected exactly under an injectivity condition. Authority is preserved only in a lax direction that discards prohibitions. Surjectivity on states yields a common abstraction without yielding equivalence. A representation theorem for tree-shaped systems shows that a filesystem and a lexical scope discipline arise from one decorated rooted tree by dual product constructions. The essay closes by separating a common abstraction from categorical equivalence, from translation of proof theories, and from computational universality, and argues that equivalence of heterogeneous formal systems is always equivalence relative to the structure that a chosen abstraction retains.

## Structure

The essay has five parts. Part I, The Mathematics of Context, introduces contexts, scope, visibility, authority, and the distinction between navigation and disclosure. Part II, Hierarchical and Computational Representations, treats filesystems and shell environments, lexical scope and syntax trees, access control, and interactive worlds as transition systems. Part III, Presheaves and Local Information, develops presheaf semantics for observation, local consistency and global reconstruction, and hidden information and observational equivalence. Part IV, Functorial Translation, studies categories of representational systems, common abstractions and forgetful functors, the relations among surjectivity, fullness, faithfulness and equivalence, translation between mathematical languages, and the limits of universality. Part V, Results and Interpretation, gives the general translation construction, what is preserved and lost under translation, and the limits of hierarchical representation.

Five appendices follow: definitions and notation, finite examples and counterexamples for visibility, disclosure and access control, worked translations among filesystem, lexical-scope and transition-system models, a formal inventory of propositions, counterexamples and open questions, and related frameworks with bibliographic notes.

## Building

The essay is a single file, `geometry_of_scope.tex`, with its bibliography included as a `thebibliography` environment, so no BibTeX run is needed. It uses the `article` class with amsmath, amssymb, amsthm, mathtools, tikz-cd, booktabs, enumitem, longtable, microtype, geometry, and hyperref. With a standard TeX Live installation, run

    pdflatex geometry_of_scope.tex
    pdflatex geometry_of_scope.tex

Two passes are needed to resolve the table of contents and cross-references.

## Status

This is a working draft, published as it is produced and revised in place. It is dedicated to the public domain.
