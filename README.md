# slavonic-typematrix

> A very opiniated Typematrix and Programmer Dvorak Oriented phonetic slavic keyboard (with an Ukrainian focus, for reasons!) XKB layout

Activate with

    setxkbmap ru -variant multilingual-typematrix

Append to your `/usr/share/X11/xkb/symbols/ru`

```
//  ; , . p y f g c r l /
//  a o e u i d h t n s -
//  ' q j k x b m w v z \

xkb_symbols "multilingual-typematrix"
{
  name[Group1] = "Slavonic phonetic Typematrix oriented";
  include "ru(winkeys)"

  key <AB01> { [ apostrophe, doublequotemark                                 ] };           // ' "
  key <AB02> { [ Cyrillic_ya,    Cyrillic_YA,  Cyrillic_dzhe,  Cyrillic_DZHE ] };           // я Я џ Џ
  key <AB03> { [ Cyrillic_shorti, Cyrillic_SHORTI,    Cyrillic_je,    Cyrillic_JE ] };      // й Й ј Ј
  key <AB04> { [ Cyrillic_ka,    Cyrillic_KA,  Macedonia_kje,  Macedonia_KJE ] };           // к К ќ Ќ
  key <AB05> { [ Cyrillic_zhe,   Cyrillic_ZHE,          U04C2,          U04C1 ] };          // ж Ж ӂ Ӂ
  key <AB06> { [ Cyrillic_be,    Cyrillic_BE                                 ] };           // б Б
  key <AB07> { [ Cyrillic_em,    Cyrillic_EM,      trademark,     registered ] };           // м М ™ ®
  key <AB08> { [ Cyrillic_sha,   Cyrillic_SHA,          U0450,          U0400 ] };          // ш Ш ѐ Ѐ
  key <AB09> { [ Cyrillic_ve,    Cyrillic_VE, Cyrillic_u_macron, Cyrillic_U_macron ] };     // в В ӯ Ӯ
  key <AB10> { [ Cyrillic_ze,    Cyrillic_ZE,  Macedonia_dse,  Macedonia_DSE ] };           // з З ѕ Ѕ
  key <AB11> { [ backslash] };                                                              // \

  key <AC01> { [ Cyrillic_a,     Cyrillic_A                                 ] };            // а А
  key <AC02> { [ Cyrillic_o,     Cyrillic_O,          U045D,          U040D ] };            // о О ѝ Ѝ
  key <AC03> { [ Cyrillic_ie,    Cyrillic_IE,   Ukrainian_ie,   Ukrainian_IE ] };           // е Е є Є
  key <AC04> { [ Cyrillic_u,     Cyrillic_U, Byelorussian_shortu, Byelorussian_SHORTU ] };  // у У ў Ў
  key <AC05> { [ Ukrainian_i,    Ukrainian_I ] };                                           // і І
  key <AC06> { [ Cyrillic_de,    Cyrillic_DE,    Serbian_dje,    Serbian_DJE ] };           // д Д ҕ Ҕ
  key <AC07> { [ Cyrillic_ha,    Cyrillic_HA,       multiply, enfilledcircbullet] };        // х Х ×
  key <AC08> { [ Cyrillic_te,    Cyrillic_TE,   Serbian_tshe,   Serbian_TSHE ] };           // т Т ћ Ћ
  key <AC09> { [ Cyrillic_en,    Cyrillic_EN,   Cyrillic_nje,   Cyrillic_NJE ] };           // н Н њ Њ
  key <AC10> { [ Cyrillic_es,    Cyrillic_ES                                 ] };           // с С
  key <AC11> { [ Cyrillic_yu,    Cyrillic_YU ] };                                           // ю Ю

  key <AD01> { [ semicolon, colon ] };                                                      // ; :
  key <AD02> { [ comma, less ] };                                                           // , <
  key <AD03> { [ period, greater ] };                                                       // . >
  key <AD04> { [ Cyrillic_pe,    Cyrillic_PE,        section,      paragraph ] };           // п П § ¶
  key <AD05> { [ Cyrillic_i, Cyrillic_I ] };                                                // и И
  key <AD06> { [ Cyrillic_ef, Cyrillic_EF, Ukrainian_ghe_with_upturn, Ukrainian_GHE_WITH_UPTURN] }; // ф Ф Ґ ґ
  key <AD07> { [ Cyrillic_ghe, Cyrillic_GHE,  Macedonia_gje, Macedonia_GJE   ] };         // г Г ѓ Ѓ
  key <AD08> { [ Cyrillic_tse, Cyrillic_TSE,      copyright                 ] };          // ц Ц ©
  key <AD09> { [ Cyrillic_er,  Cyrillic_ER, Cyrillic_i_macron, Cyrillic_I_macron ] };     // р Р ӣ Ӣ
  key <AD10> { [ Cyrillic_el,    Cyrillic_EL,   Cyrillic_lje,   Cyrillic_LJE ] };         // л Л љ Љ
  key <AD11> { [ slash, question ] };                                                     // / ?
  key <AD12> { [ at ] };                                                                  // @

  // key <AC10> { [   Cyrillic_che,   Cyrillic_CHE,       ellipsis, degree         ] }; // ч Ч … °
  // key <AC11> { [ Cyrillic_softsign, Cyrillic_SOFTSIGN, rightsinglequotemark, hyphen ] }; // ь Ь '
  // key <TLDE> { [ Cyrillic_hardsign, Cyrillic_HARDSIGN, guillemotleft, U2039     ] }; // ъ Ъ « ‹
  // key <AD06> { [  Cyrillic_yeru,  Cyrillic_YERU,   Ukrainian_yi,   Ukrainian_YI ] }; // ы Ы ї Ї
  // key <AD12> { [     Cyrillic_e,     Cyrillic_E,   bracketright,     braceright ] }; // э Э ] }
  // key <AE12> { [ Cyrillic_shcha, Cyrillic_SHCHA,       equal,         plusminus ] }; // щ Щ = ±
  // key <BKSL> { [    Cyrillic_io,    Cyrillic_IO,      backslash,            bar ] }; // ё Ё / |

  // key <AD11> { [ bracketleft,      braceleft ] };                                  //  [ {
  // key <AE01> { [ NoSymbol,       NoSymbol, guillemotright,     U203A ] };          //   » ›
  // key <AE03> { [ NoSymbol,       NoSymbol,     numbersign,     dead_grave ] };     // #
  // key <AE04> { [ NoSymbol,         dollar,       EuroSign,  dead_doublegrave  ] }; // $ €
  // key <AE05> { [ NoSymbol,       NoSymbol,          U20B4,     dead_macron ] };    // ₴
  // key <AE06> { [ NoSymbol,     apostrophe,     asciitilde, dead_circumflex    ] }; //  ' ~
  // key <AE07> { [ NoSymbol,      ampersand,      plus, dead_inverted_breve    ] };  //  & +
  // key <LSGT> {[  backslash,            bar                                 ] };    // \ |
};
