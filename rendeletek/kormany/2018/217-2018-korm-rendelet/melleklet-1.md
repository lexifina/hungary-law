1. melléklet a 217/2018. (XI. 27.) Korm. rendelethez

„8. melléklet a 218/2009. (X. 6.) Korm. rendelethez

A megyei területrendezési tervek téradat-rétegeinek műszaki követelményei és jelkulcsa

1. Térségi szerkezeti terv

|  | A | B | C | D | E | F | G | H | I | J |

| 1. | Réteg | Attribútum adatok | Jelkulcs |

| 2. | Objektum kód/ rétegnév | Objektum típus | Objektum megjelenése | Típus-specifikus tulajdonságok | Oszlopnév | Adat-típus | Értékkészlet | Objektum megjelenítési módja | Objektum színe |

| 3. | tersegi_teruletfel- hasznalasi_kate- goriak | Térségi terület- felhasználási kategóriák | poligon | Kategória | KATEGORIA | string | erdo_t | Erdőgazdálkodási térség |  | R:101 G:168 B:67 |

| 4. | mg_t | Mezőgazdasági térség |  | R:255 G:255 B:217 |

| 5. | vg_t | Vízgazdálkodási térség |  |  | R:166 G:234 B:255 |

| 6. | t_t | Települési térség |  | R:178 G:178 B:178 |

| 7. | s_t | Sajátos területfelhasználású térség |  | R:115 G:38 B:0 |

| 8. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 9. | telepules_rendszer_ elemei | Településrendszer elemei | pont | Kategória | KATEGORIA | string | rtk | Regionális térszervező központ |  | R:0 G:0 B:0 (12pt) R:130 G:130 B:130 (16pt) R:0 G:0 B:0 (20pt) |

| 10. | ttk | Térségi térszervező központ |  | R:0 G:0 B:0 (10pt) R:130 G:130 B:130 (14pt) |

| 11. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 12. | gyorsforgalmi_ut | Gyorsforgalmi út | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 (5pt) R:255 G:255 B:255 (1pt) |

| 13. | 0 | Tervezett |  | R:255 G:0 B:0 (5pt) R:255 G:255 B:255 (1pt) |

| 14. | Elem száma | UTSZAM | string |  | "M" + szám: pl. M19 |  |  |

| 15. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Bőny (M1) - Győr (1. sz. főút) |  |  |

| 16. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 17. | fout | Főút | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 (3pt) |

| 18. | 0 | Tervezett |  | R:255 G:0 B:0 (5pt) R:0 G:0 B:0 (3pt) |

| 19. | Elem száma | UTSZAM | string |  | "R" + szám pl. R21 vagy szám pl. 73 |  |  |

| 20. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Csopak (71. sz. főút) - Veszprém (8. sz. főút) |  |  |

| 21. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 22. | nagysebessegu_ vasutvonal | Nagysebességű vasútvonal | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:255 G:255 B:0 (2pt) R:0 G:0 B:0 (4pt) |

| 23. | 0 | Tervezett |  | R:255 G:255 B:0 (2pt) R:255 G:0 B:0 (4pt) |

| 24. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. (Ausztria és Szlovákia) – Hegyeshalom térsége és Rajka térsége – Budapest [XI. kerület, Kelenföld] – Budapest [Budapest Liszt Ferenc Nemzetközi Repülőtér] – Röszke és Kübekháza – (Szerbia és Románia) |  |  |

| 25. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 26. | egyeb_orszagos_ torzshalozati_ vasuti_palya | Egyéb országos törzshálózati vasúti pálya | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:155 G:187 B:89 (2pt) R:0 G:0 B:0 (4pt) |

| 27. | 0 | Tervezett |  | R:155 G:187 B:89 (2pt) R:255 G:0 B:0 (4pt) |

| 28. | Elem száma | VONALSZAM | integer |  | szám pl. 9 |  |  |

| 29. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Fertőszentmiklós – (Ausztria) |  |  |

| 30. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 31. | nemzetkozi_ kereskedelmi_ repuloter | Nemzetközi kereskedelmi repülőtér | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:255 G:255 B:0 R:0 G:0 B:0 (14pt) |

| 32. | 0 | Tervezett |  | R:255 G:255 B:0 R:255 G:0 B:0 (14pt) |

| 33. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Debrecen [Debreceni Nemzetközi Repülőtér] |  |  |

| 34. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 35. | kozos_felhasznalasu_katonai_es_polgari_ repuloterre_fej- lesztheto_repuloter | Közös felhasználású katonai és polgári repülőtérré fejleszthető repülőtér | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:155 G:187 B:89 R:0 G:0 B:0 (14pt) |

| 36. | 0 | Tervezett |  | R:155 G:187 B:89 R:255 G:0 B:0 (14pt) |

| 37. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Pápa |  |  |

| 38. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 39. | orszagos_kerekpar- utvonal | Országos kerékpárút-vonal | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 (5pt) |

| 40. | 0 | Tervezett |  | R:255 G:0 B:0 (1pt) R:0 G:0 B:0 (5pt) |

| 41. | Elem száma | UTSZAM | string |  | Szám pl. 2.D |  |  |

| 42. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Nagybárkány – Márkháza – Nagykeresztúr – Salgótarján – Somoskőújfalu – (Szlovákia) |  |  |

| 43. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 44. | orszagos_kikoto | Országos kikötő | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:255 G:255 B:0 R:0 G:0 B:0 (14pt) |

| 45. | 0 | Tervezett |  | R:255 G:255 B:0 R:255 G:0 B:0 (14pt) |

| 46. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Baja |  |  |

| 47. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 48. | hatarkikoto | Határkikötő | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:155 G:187 B:89 R:0 G:0 B:0 (14pt) |

| 49. | 0 | Tervezett |  | R:155 G:187 B:89 R:255 G:0 B:0 (14pt) |

| 50. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Szeged |  |  |

| 51. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 52. | atomeromu | Atomerőmű | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 53. | 0 | Tervezett |  | R:255 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 54. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Paks |  |  |

| 55. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 56. | egyeb_50mw_vagy_ annal_nagyobb_ nevleges_teljesito- kepessegu_eromu | Egyéb 50MW vagy annál nagyobb névleges teljesítő- képességű erőmű | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 57. | 0 | Tervezett |  | R:255 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 58. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Visonta |  |  |

| 59. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 60. | atviteli_halozati_ tavvezetek_ 750_kvos | 750 kV-os átviteli hálózati távvezeték | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:197 G:0 B:255 (3pt) |

| 61. | 0 | Tervezett |  | R:197 G:0 B:255 (3pt) R:255 G:0 B:0 (5pt) |

| 62. | Elem száma | AG_SZAM | string |  | Szám/számok: pl. 1. |  |  |

| 63. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Albertirsa – Szolnok – Hajdúböszörmény – Kisvárda térsége – Barabás – (Ukrajna) |  |  |

| 64. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 65. | atviteli_halozati_ tavvezetek_ 400_kvos | 400 kV-os átviteli hálózati távvezeték | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:197 G:0 B:255 (1,5pt) |

| 66. | 0 | Tervezett |  | R:197 G:0 B:255 (1,5pt) R:255 G:0 B:0 (3,5pt) |

| 67. | Elem száma | AG_SZAM | string |  | Szám/számok: pl. 26., 27. |  |  |

| 68. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Martonvásár – Perkáta – Paks |  |  |

| 69. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 70. | atviteli_halozati_tavvezetek_220_kvos | 220 kV-os átviteli hálózati távvezeték | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:197 G:0 B:255 (1pt és 5pt) |

| 71. | 0 | Tervezett |  | R:197 G:0 B:255 (1pt) R:255 G:0 B:0 (5pt) |

| 72. | Elem száma | AG_SZAM | string |  | Szám/számok: pl. 70., 71. |  |  |

| 73. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Nagyút – Mezőtárkány – Sajószöged |  |  |

| 74. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 75. | foldgazszallito_ vezetek | Földgázszállító vezeték | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:137 G:90 B:68 (1,5pt) |

| 76. | 0 | Tervezett |  | R:137 G:90 B:68 (1,5pt) R:255 G:0 B:0 (3,5pt) |

| 77. | Elem száma/elnevezése | AG_SZAM | string |  | Szám: pl. 100-01 |  |  |

| 78. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Beregdaróc – Tarpa – Nagyar |  |  |

| 79. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 80. | koolajszallito_ vezetek | Kőolajszállító vezeték | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:155 G:187 B:89 (1,5pt) |

| 81. | 0 | Tervezett |  | R:155 G:187 B:89 (1,5pt) R:255 G:0 B:0 (3,5pt) |

| 82. | Elem elnevezése | NEV | string |  | Elnevezés: pl. Adria |  |  |

| 83. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Százhalombatta – Káloz – Kára – Kutas – Berzence – (Horvátország) |  |  |

| 84. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 85. | termekvezetek | Termékvezeték | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:205 G:170 B:102 (1,5pt) |

| 86. | 0 | Tervezett |  | R:205 G:170 B:102 (1,5pt) R:255 G:0 B:0 (3,5pt) |

| 87. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Százhalombatta – Kápolnásnyék |  |  |

| 88. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 89. | vtt_tarozo | VTT-tározó | poligon | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:77 B:168 (outline: 0,5pt, line: 0,5pt) |

| 90. | 0 | Tervezett |  | R:255 G:0 B:0 (outline: 0,5pt, line: 0,5pt) |

| 91. | Elem elnevezése | NEV | string |  | Elnevezés: pl. Cigánd-Tiszakarádi |  |  |

| 92. | Főbb érintett települések | TELEP | string |  | Települések neve: pl. Nagyrozvágy, Cigánd, Pácin |  |  |

| 93. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 94. | orszagos_vizkarel- haritasi_celu_tarozo | Országos vízkár- elhárítási célú tározó | poligon | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:77 B:168 (outline: 1pt, line: 0,5 és 1pt) |

| 95. | 0 | Tervezett |  | R:255 G:0 B:0 (outline: 1pt, line: 0,5 és 1pt) |

| 96. | Elem elnevezése | NEV | string |  | Elnevezés: pl. Mérgesi |  |  |

| 97. | Főbb érintett települések | TELEP | string |  | Települések neve: pl. Köröstarcsa, Körösladány |  |  |

| 98. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 99. | kiemelt_jelento- segu_vizi_epitmeny | Kiemelt jelentőségű vízi építmény | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 100. | 0 | Tervezett |  | R:255 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 101. | Elem elnevezése | NEV | string |  | Elnevezés: pl. Kiskörei vízlépcső |  |  |

| 102. | Főbb érintett települések | TELEP | string |  | Települések neve: pl. Abádszalók, Kisköre |  |  |

| 103. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 104. | orszagos_jelento- segu_csatorna | Országos jelentőségű csatorna | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:77 B:168 (2pt) |

| 105. | 0 | Tervezett |  | R:0 G:77 B:168 (2pt) R:255 G:0 B:0 (4pt) |

| 106. | Elem elnevezése | NEV | string |  | Elnevezés: pl. Nagy-foki-csatorna |  |  |

| 107. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Szeghalom–Újiráz/Komádi |  |  |

| 108. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 109. | elsorendu_arvizve- delmi_fovedvonal | Elsőrendű árvíz- védelmi fővédvonal | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 (1 és 3pt) |

| 110. | 0 | Tervezett |  | R:255 G:0 B:0 (1 és 3pt) |

| 111. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 112. | veszelyeshulladek_ lerako | Veszélyeshulladék- lerakó | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:255 G:0 B:0 R:0 G:0 B:0 (14pt) |

| 113. | 0 | Tervezett |  | R:255 G:0 B:0 R:155 G:187 B:89 (14pt) |

| 114. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Marcali |  |  |

| 115. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 116. | veszelyeshulladek- egeto_mu | Veszélyeshulladék- égető mű | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 R:255 G:0 B:0 (14pt) |

| 117. | 0 | Tervezett |  | R:155 G:187 B:89 R:255 G:0 B:0 (14pt) |

| 118. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Királyszentistván |  |  |

| 119. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 120. | radioaktivhulladek_ tarolo | Radioaktív- hulladék-tároló | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:255 G:255 B:0 R:0 G:0 B:0 (14pt) |

| 121. | 0 | Tervezett |  | R:255 G:255 B:0 R:255 G:0 B:0 (14pt) |

| 122. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Bátaapáti |  |  |

| 123. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 124. | tersegi_szerepu_ osszekoto_ut | Térségi szerepű összekötő út | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:255 G:255 B:0 (1pt) R:0 G:0 B:0 (2pt) |

| 125. | 0 | Tervezett |  | R:255 G:255 B:0 (1pt) R:255 G:0 B:0 (2pt) |

| 126. | Elem száma | UTSZAM | integer |  | Szám: pl. 1457 |  |  |

| 127. | Főbb érintett települések | TELEP | string |  | Települések lánca: Tárnok (7.sz. főút) – Herceghalom (1.sz. főút) |  |  |

| 128. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 129. | mellekut | Mellékút | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 (1pt) R:255 G:255 B:255 (0,5pt) |

| 130. | 0 | Tervezett |  | R:255 G:0 B:0 (1pt) R:255 G:255 B:255 (0,5pt) |

| 131. | Elem száma | UTSZAM | integer |  | Szám: pl. 1457 |  |  |

| 132. | Főbb érintett települések | TELEP | string |  | Települések lánca: Tikos - Szegerdő |  |  |

| 133. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 134. | orszagos_vasuti_ mellekvonal | Országos vasúti mellékvonal | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 (2pt) R:255 G:255 B:255 (1pt) |

| 135. | 0 | Tervezett |  | R:255 G:0 B:0 (2pt) R:255 G:255 B:255 (1pt) |

| 136. | Elem száma | VONALSZAM | string |  | Szám: pl. 23 |  |  |

| 137. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Zalaegerszeg - Rédics |  |  |

| 138. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 139. | tersegi_repuloter | Térségi repülőtér | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 140. | 0 | Tervezett |  | R:255 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 141. | Főbb érintett települések | TELEP | string |  | Település név: Szentkirályszabadja |  |  |

| 142. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 143. | tersegi_kerekpar- utvonal | Térségi kerékpárút- vonal | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:155 G:187 B:89 (3pt) |

| 144. | 0 | Tervezett |  | R:155 G:187 B:89 (3pt) R:255 G:0 B:0 (1pt) |

| 145. | Főbb érintett települések | TELEP | string |  | Települések lánca: Lulla - Tab |  |  |

| 146. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 147. | tersegi_kikoto | Térségi kikötő | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 148. | 0 | Tervezett |  | R:255 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 149. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Csopak |  |  |

| 150. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 151. | kompatkelohely | Kompátkelőhely | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 152. | 0 | Tervezett |  | R:255 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 153. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Szántód - Tihany |  |  |

| 154. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 155. | tersegi_logisztikai_ kozpont | Térségi logisztikai központ | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 156. | 0 | Tervezett |  | R:255 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 157. | Főbb érintett települések | TELEP | string |  | Település neve |  |  |

| 158. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 159. | eromu _ 5_50_mw_nevleges _teljesitokepessegu_ | 5-50 MW névleges teljesítőképességű erőmű | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 160. | 0 | Tervezett |  | R:255 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 161. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Kulcs |  |  |

| 162. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 163. | atvitelt_befolya- solo_132_kvos_ eloszto_halozat | Átvitelt befolyásoló 132 kV-os elosztó hálózat | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:197 G:0 B:255 (1,5pt) |

| 164. | 0 | Tervezett |  | R:197 G:0 B:255 (1,5pt) R:255 G:0 B:0 (1pt) |

| 165. | Elem száma | AGAZATISZAM | string |  | Szám: pl. 123 |  |  |

| 166. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Kecskemét - Izsák |  |  |

| 167. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 168. | tersegi_ellatast_ biztosito_132_kvos_ eloszto_halozat | Térségi ellátást biztosító 132 kV-os elosztó hálózat | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:197 G:0 B:255 (0,5 és 1pt) |

| 169. | 0 | Tervezett |  | R:197 G:0 B:255 (1pt) R:255 G:0 B:0 (0,5pt) |

| 170. | Elem száma | AGAZATISZAM | string |  | Szám: pl. 123-01 |  |  |

| 171. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Kecskemét - Izsák |  |  |

| 172. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 173. | foldgazeloszto_ vezetek | Földgázelosztó vezeték | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:137 G:90 B:68 (1,5pt) |

| 174. | 0 | Tervezett |  | R:137 G:90 B:68 (1,5pt) R:255 G:0 B:0 (1pt) |

| 175. | Elem száma/elnevezése | AGAZATISZAM | string |  | Szám: pl. 145-02 |  |  |

| 176. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Sopron - Újkér |  |  |

| 177. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 178. | tarozo_1_millio_m3t_meghalado_ terfogatu_vizkar- elharitasi_celu | 1 millió m3-t meghaladó térfogatú vízkár- elhárítási célú tározó | poligon | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:77 B:168 (outline: 0,5pt, line: 0,5pt) |

| 179. | 0 | Tervezett |  | R:255 G:0 B:0 (outline: 0,5pt, line: 0,5pt) |

| 180. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Sopron |  |  |

| 181. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 182. | tersegi_csatorna | Térségi csatorna | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:77 B:168 (1,5pt) |

| 183. | 0 | Tervezett |  | R:0 G:77 B:168 (1,5pt) R:255 G:0 B:0 (1pt) |

| 184. | Főbb érintett települések | TELEP | string |  | Települések lánca: pl. Osli - Kapuvár |  |  |

| 185. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 186. | masodrendu_arviz- vedelmi_fovedvonal | Másodrendű árvíz- védelmi fővédvonal | vonal | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:130 G:130 B:130 (1 és 3pt) |

| 187. | 0 | Tervezett |  | R:130 G:130 B:130 (1pt) R:255 G:0 B:0 (3pt) |

| 188. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

| 189. | tersegi_hulladek- kezelo | Térségi hulladék- kezelő | pont | Meglévő vagy tervezett? | MEGLEVO | integer | 1 | Meglévő |  | R:0 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 190. |  | 0 | Tervezett |  | R:255 G:0 B:0 R:255 G:255 B:255 (14pt) |

| 191. | Főbb érintett települések | TELEP | string |  | Település neve: pl. Szolnok |  |  |

| 192. | Elfogadó jogszabály száma | ELF_JOGSZ | string |  | pl. 12/2010. megyei önkorm. rendelet |  |  |

2. Térségi övezetek
