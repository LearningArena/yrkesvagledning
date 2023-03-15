
# AF JobAd Enrichments

[Description](https://jobtechdev.se/sv/komponenter/jobad-enrichments)

[Getting started](https://github.com/Jobtechdev-content/JobAdEnrichments-content/blob/master/GettingstartedJobAdEnrichmentsSE.md)


## Some useful examples

### enrichtextdocuments

##### Input
```
  ...
      "doc_headline": "Sjuksköterska",
      "doc_text": "Vi letar efter en empatisk sjuksköterska. Du ska vara noggrann, kreativ och jätteglad. Krav: sjuksköterskelegitimation och ha erfarenhet av akutsjukvård. Du kommer att arbeta i Stockholm."
  ...
```

##### Output
```json
"enriched_candidates": {
    "occupations": [
        {
            "concept_label": "Sjuksköterska",
            "term": "sjuksköterska",
            "prediction": 0.605962932
        },
        {
            "concept_label": "Sjuksköterska",
            "term": "sjuksköterska",
            "prediction": 0.884523898
        }
    ],
    "competencies": [
        {
            "concept_label": "Sjuksköterskelegitimation",
            "term": "sjuksköterskelegitimation",
            "prediction": 0.9965306818
        },
        {
            "concept_label": "Akutsjukvård",
            "term": "akutsjukvård",
            "prediction": 0.9954738915
        }
    ],
    "traits": [
        {
            "concept_label": "Empatisk",
            "term": "empatisk",
            "prediction": 0.521104693
        },
        {
            "concept_label": "Noggrann",
            "term": "noggrann",
            "prediction": 0.911307693
        },
        {
            "concept_label": "Kreativ",
            "term": "kreativ",
            "prediction": 0.931879282
        }
    ],
    "geos": [
        {
            "concept_label": "Stockholm",
            "term": "stockholm",
            "prediction": 0.910521507
        }
    ]
}
```
}