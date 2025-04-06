---
title: "Functions Supported for Set of Annotations Data"
weight: 1
---


# Functions Supported for Set of Annotations Data

*   **annotatedRegions** (Sequence seq, AnnotationTable anns, QString name) — returns subsequences of the annotations with the specified “name”.
*   **addQualifier** (AnnotationTable anns, QString qual, QString val, QString name = “”) — sets the qualifier in the annotations with the specified “name” to the specified value. If the “name” is not specified, then all annotations are taken into account.
*   **getLocation** (AnnotationTable anns, int ind) — returns the annotation location with the specified index.
*   **filterByQualifier** (AnnotationsTable anns, QString qual, QString val) - returns the qualifier with the specified value.
*   **hasAnnotationName** \- (AnnotationsTable anns, QString " ") - returns the annotation with the specified name there is or there is not.
