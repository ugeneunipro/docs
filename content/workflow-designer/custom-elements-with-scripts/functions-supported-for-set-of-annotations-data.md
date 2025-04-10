---
title: "Functions Supported for Set of Annotations Data"
weight: 300
---

# Functions Supported for Set of Annotations Data

*   **annotatedRegions** (Sequence seq, AnnotationTable anns, QString name) — returns subsequences of the annotations with the specified “name”.
*   **addQualifier** (AnnotationTable anns, QString qual, QString val, QString name = “”) — sets the qualifier in the annotations with the specified “name” to the specified value. If the “name” is not specified, then all annotations are taken into account.
*   **getLocation** (AnnotationTable anns, int ind) — returns the annotation location with the specified index.
*   **filterByQualifier** (AnnotationTable anns, QString qual, QString val) — returns the qualifier with the specified value.
*   **hasAnnotationName** (AnnotationTable anns, QString " ") — checks if there is an annotation with the specified name.