
# AF Atlas Taxonomy

[Web interface](https://atlas.jobtechdev.se/)

[Relational diagram](https://atlas.jobtechdev.se/page/about.html)

[API](https://taxonomy.api.jobtechdev.se/v1/taxonomy/swagger-ui/index.html)

## Some useful examples

- Skills
  - [Client, programmering/Server, programmering](https://atlas.jobtechdev.se/page/taxonomy.html#concept=Bw3F_U6s_ZeC)
- Occupations
  - [Skådespelare](https://atlas.jobtechdev.se/page/taxonomy.html#concept=iBUL_s38_izZ)
- Education field
  - [Hälso- och sjukvård, allmän utbildning](https://atlas.jobtechdev.se/page/taxonomy.html#concept=Tqh5_xkL_G7L)

## API test

<details>
<summary>See answer for call to autocomplete endpoint, using 'svetsning' as search string and 'skill' as type</summary>

```

[
    {
        "taxonomy/id": "ynW8_Jr4_5tT",
        "taxonomy/type": "skill",
        "taxonomy/preferred-label": "Svetsning och lödning, VVS"
    },
    {
        "taxonomy/id": "Znb9_xEs_YKm",
        "taxonomy/type": "skill",
        "taxonomy/preferred-label": "EN 287-1, 131 MIG-svetsning/ISO 9606-1"
    },
    {
        "taxonomy/id": "7kqy_wX6_gEP",
        "taxonomy/type": "skill",
        "taxonomy/preferred-label": "EN 287-1, 135 MAG-svetsning/ISO 9606-1"
    },
    {
        "taxonomy/id": "5x8K_uya_8pn",
        "taxonomy/type": "skill",
        "taxonomy/preferred-label": "EN 287-1, 141 TIG-svetsning/ISO 9606-1"
    },
    {
        "taxonomy/id": "Yzer_FdZ_Li2",
        "taxonomy/type": "skill",
        "taxonomy/preferred-label": "EN 287-1, 136 MAG-svetsning med slaggande rörelektrod/ISO 9606-1"
    },
    {
        "taxonomy/id": "F6sW_dXF_fba",
        "taxonomy/type": "skill",
        "taxonomy/preferred-label": "EN 287-1, 138 MAG-svetsning med metallpulverfylld rörelektrod/ISO 9606-1"
    },
    {
        "taxonomy/id": "1ym6_zNX_hkG",
        "taxonomy/type": "skill",
        "taxonomy/preferred-label": "EN 1418, Robotsvetsning/ISO 14732, Mekaniserad svetsning"
    },
    {
        "taxonomy/id": "hrB3_BBp_XH3",
        "taxonomy/type": "skill",
        "taxonomy/preferred-label": "ISO 9606-2, 131 MIG-svetsning"
    },
    {
        "taxonomy/id": "3ugi_rtr_nWB",
        "taxonomy/type": "skill",
        "taxonomy/preferred-label": "ISO 9606-2, 141 TIG-svetsning"
    },
    {
        "taxonomy/id": "FfhY_CoE_CpR",
        "taxonomy/type": "skill",
        "taxonomy/preferred-label": "Mekaniserad svetsning"
    },
    {
        "taxonomy/id": "Z7Yj_NjR_9EQ",
        "taxonomy/type": "skill",
        "taxonomy/preferred-label": "MAG-svetsning med rörelektrod"
    },
    {
        "taxonomy/id": "Q1D1_Pdc_rnT",
        "taxonomy/type": "skill",
        "taxonomy/preferred-label": "MIG-svetsning"
    },
    {
        "taxonomy/id": "NH9n_Snj_CNM",
        "taxonomy/type": "skill",
        "taxonomy/preferred-label": "MAG-svetsning"
    },
    {
        "taxonomy/id": "WBnc_JXj_MvY",
        "taxonomy/type": "skill",
        "taxonomy/preferred-label": "TIG-svetsning"
    }
]

```

</details>
