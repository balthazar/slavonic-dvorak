# slavonic-dvorak

> A very opiniated Dvorak Oriented phonetic slavic keyboard (with an Ukrainian focus, because we all know Russia is just one big Ukrainian province) XKB layout

```
& [ { } ( = * ) + ] ! ?@
щ ё . п и ф г ц р л ч
а о е у і д х т н с ю
ь я й к ж б м ш в з э
```

### Notes

- Numbers & non-chars follow the Programmer Dvorak standard, and could cause you to go insane
- Upper-row non-chars could potentially be replaced to more useful ones for text purposes rather than dev

```
// semicolon colon numbersign apostrophe backslash, slash, less, greater, bar, dollar
// ; : # ' \ / < > | $
```

### Activation

    setxkbmap ru -variant multilingual-typematrix

### Installation

Append the following to your `/usr/share/X11/xkb/symbols/ru`:

```
xkb_symbols "slavonic-dvorak"
{
  name[Group1] = "Slavonic phonetic Dvorak oriented";
  include "ru(winkeys)"

  key <AE01> { [ ampersand,    percent ] }; // & %
  key <AE02> { [ bracketleft,  7       ] }; // [ 7
  key <AE03> { [ braceleft,    5       ] }; // { 5
  key <AE04> { [ braceright,   3       ] }; // } 3
  key <AE05> { [ parenleft,    1       ] }; // ( 1
  key <AE06> { [ equal,        9       ] }; // = 9
  key <AE07> { [ asterisk,     0       ] }; // * 0
  key <AE08> { [ parenright,   2       ] }; // ) 2
  key <AE09> { [ plus,         4       ] }; // + 4
  key <AE10> { [ bracketright, 6       ] }; // ] 6
  key <AE11> { [ exclam,       8       ] }; // ! 8
  key <AE12> { [ question,     at      ] }; // ? @

  key <AD01> { [ Cyrillic_shcha, Cyrillic_SHCHA                                                     ] }; // щ Щ
  key <AD02> { [ Cyrillic_io,    Cyrillic_IO                                                        ] }; // ё Ё
  key <AD03> { [ period,         comma                                                              ] }; // . ,
  key <AD04> { [ Cyrillic_pe,    Cyrillic_PE                                                        ] }; // п П
  key <AD05> { [ Cyrillic_i,     Cyrillic_I                                                         ] }; // и И
  key <AD06> { [ Cyrillic_ef,    Cyrillic_EF,  Macedonia_gje,             Macedonia_GJE             ] }; // ф Ф ѓ Ѓ
  key <AD07> { [ Cyrillic_ghe,   Cyrillic_GHE, Ukrainian_ghe_with_upturn, Ukrainian_GHE_WITH_UPTURN ] }; // г Г Ґ ґ
  key <AD08> { [ Cyrillic_tse,   Cyrillic_TSE                                                       ] }; // ц Ц
  key <AD09> { [ Cyrillic_er,    Cyrillic_ER,  Cyrillic_i_macron,         Cyrillic_I_macron         ] }; // р Р ӣ Ӣ
  key <AD10> { [ Cyrillic_el,    Cyrillic_EL,  Cyrillic_lje,              Cyrillic_LJE              ] }; // л Л љ Љ
  key <AD11> { [ Cyrillic_che,   Cyrillic_CHE                                                       ] }; // ч Ч

  key <AC01> { [ Cyrillic_a,  Cyrillic_A                                            ] }; // а А
  key <AC02> { [ Cyrillic_o,  Cyrillic_O,  U045D,               U040D               ] }; // о О ѝ Ѝ
  key <AC03> { [ Cyrillic_ie, Cyrillic_IE, Ukrainian_ie,        Ukrainian_IE        ] }; // е Е є Є
  key <AC04> { [ Cyrillic_u,  Cyrillic_U,  Byelorussian_shortu, Byelorussian_SHORTU ] }; // у У ў Ў
  key <AC05> { [ Ukrainian_i, Ukrainian_I, Ukrainian_yi,        Ukrainian_YI        ] }; // і І ї Ї
  key <AC06> { [ Cyrillic_de, Cyrillic_DE, Serbian_dje,         Serbian_DJE         ] }; // д Д ҕ Ҕ
  key <AC07> { [ Cyrillic_ha, Cyrillic_HA, multiply                                 ] }; // х Х ×
  key <AC08> { [ Cyrillic_te, Cyrillic_TE, Serbian_tshe,        Serbian_TSHE        ] }; // т Т ћ Ћ
  key <AC09> { [ Cyrillic_en, Cyrillic_EN, Cyrillic_nje,        Cyrillic_NJE        ] }; // н Н њ Њ
  key <AC10> { [ Cyrillic_es, Cyrillic_ES                                           ] }; // с С
  key <AC11> { [ Cyrillic_yu, Cyrillic_YU                                           ] }; // ю Ю

  key <AB01> { [ Cyrillic_softsign, Cyrillic_hardsign, Cyrillic_yeru,     Cyrillic_YERU     ] }; // ь ъ ы Ы
  key <AB02> { [ Cyrillic_ya,       Cyrillic_YA,       Cyrillic_dzhe,     Cyrillic_DZHE     ] }; // я Я џ Џ
  key <AB03> { [ Cyrillic_shorti,   Cyrillic_SHORTI,   Cyrillic_je,       Cyrillic_JE       ] }; // й Й ј Ј
  key <AB04> { [ Cyrillic_ka,       Cyrillic_KA,       Macedonia_kje,     Macedonia_KJE     ] }; // к К ќ Ќ
  key <AB05> { [ Cyrillic_zhe,      Cyrillic_ZHE,      U04C2,             U04C1             ] }; // ж Ж ӂ Ӂ
  key <AB06> { [ Cyrillic_be,       Cyrillic_BE                                             ] }; // б Б
  key <AB07> { [ Cyrillic_em,       Cyrillic_EM                                             ] }; // м М
  key <AB08> { [ Cyrillic_sha,      Cyrillic_SHA,      U0450,             U0400             ] }; // ш Ш ѐ Ѐ
  key <AB09> { [ Cyrillic_ve,       Cyrillic_VE,       Cyrillic_u_macron, Cyrillic_U_macron ] }; // в В ӯ Ӯ
  key <AB10> { [ Cyrillic_ze,       Cyrillic_ZE,       Macedonia_dse,     Macedonia_DSE     ] }; // з З ѕ Ѕ
  key <AB11> { [ Cyrillic_e,        Cyrillic_E                                              ] }; // э Э
};
```
