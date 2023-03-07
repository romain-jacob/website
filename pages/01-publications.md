---
layout: single
permalink: /publications
---

# Selected publications

> If you _really_ want full lists, you can check my [ORCID](https://orcid.org/0000-0002-2218-5750) or [Google Scholar](https://scholar.google.com/citations?user=O74-HUUAAAAJ&hl=en) profiles.

{% bibliography --file Selected %}


<!-- FUNCTION {format.names}
{ 's :=
  #1 'nameptr :=
  s num.names$ 'numnames :=
  numnames 'namesleft :=
    { namesleft #0 > }
    { s nameptr "{ff~}{vv~}{ll}{, jj}" format.name$ 't :=
      nameptr #1 >
        { namesleft #1 >
            { ", " * t * }
            { numnames #2 >
                { "," * }
                'skip$
              if$
              t "others" =
                { " et~al." * }
                { " and " * t * }
              if$
            }
          if$
        }
        't
      if$
      nameptr #1 + 'nameptr :=
      namesleft #1 - 'namesleft :=
    }
  while$
} -->