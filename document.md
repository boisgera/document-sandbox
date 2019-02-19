% Titre du Document
% Auteur 1; Auteur 2
% Date

Premier Pas
--------------------------------------------------------------------------------

Se reporter par exemple à <https://commonmark.org/> pour une courte introduction 
au format Markdown. 

Il existe de multiples variantes de ce format, plus ou moins (in-)compatibles.
La variante (*flavor*) de Markdown utilisée dans ce document est celle
exploitée par [pandoc]. Elle permet notamment d'intégrer des formules 
mathématiques au texte, une bibliographie, etc.  
C'est aussi le format utilisé pour la partie texte de [R Markdown][R-MD].
Pandoc -- le logiciel -- à le mérite de supporter de nombreux
formats de sortie (PDF, HTML, ODT, etc.) *out-of-the-box* et
d'être largement configurable[^note-API]. 

[^note-API]: Avec [un modèle de document][DOM]
  simple et spécifié formellement et un support logiciel adapté, 
  il se prête particulièrement bien à l'analyse et la
  transformation automatique de document requis pour des usages avancés.


[pandoc]: https://pandoc.org/MANUAL.html
[DOM]: http://hackage.haskell.org/package/pandoc-types-1.19/docs/Text-Pandoc-Definition.html
[R-MD]: https://bookdown.org/yihui/rmarkdown/markdown-syntax.html



Bibliographie
--------------------------------------------------------------------------------

La bibliographie peut être définie au format [CSL-JSON],
qui a la structure suivante:

    [
      {
        "id": "Knuth92",
        "type": "article-journal",
        "title": "Two notes on notation.",
        "container-title": "American Mathematical Monthly",
        "page": "403–422",
        "volume": "99",
        "issue": "5",
        "ISSN": "0002-9890",
        "journalAbbreviation": "Am. Math. Mon.",
        "language": "English",
        "author": 
          [
            {
              "family": "Knuth",
              "given": "Donald E."
            }
          ],
        "issued": 
          {
            "date-parts": [["1992"]]
          }
      }
    ]

Le schéma décrivant en détail le format peut être trouvé [ici][CSL-Data].
Le cas échéant, des outils comme [Zotero] peuvent assurer la conversion
d'autres formats, comme BibTex, vers CSL-JSON.

Les documents de la bibliographie peuvent ensuite être cités comme suit:

    Ca donne toujours de la crédibilité de citer [@Knuth92]

Le résultat: "Ca donne toujours de la crédibilité de citer [@Knuth92]".

**Référence:** <https://pandoc.org/MANUAL.html#citations>


[CSL-JSON]: https://github.com/citation-style-language/schema
[Zotero]: https://www.zotero.org/
[CSL-Data]: https://github.com/citation-style-language/schema/blob/master/csl-data.json


--------------------------------------------------------------------------------

Bac à Sable
================================================================================


Section (niveau 2)
--------------------------------------------------------------------------------

### Section (niveau 3)

Formules *inline* -- $a=1$ -- ou *display*:

$$
\int_0^1 f(x) \, dx
$$

*Italique*, **Gras**.

Liste:

  - ...
  - ...
  - ...

--------------------------------------------------------------------------------

Section "typée"
--------------------------------------------------------------------------------

### Théorème fondamental du calcul {.theorem}

Pour toute fonction dérivable $f: [a,b] \to \mathbb{R}^m,$
  
  $$
  f(b) = f(a) + \int_a^b f'(t) \, dt.
  $$



Bibliographie
================================================================================