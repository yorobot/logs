# cache worldfootball (wfb) datsets in Football.TXT




## tips & tricks


### step 1 - tokens/tokenizer

to double check on syntax and more try:

    $ fbtok . -q        #  use -q/--quiet

resulting in:

    OK   no parse errors found in 281 datafile(s)

### step 2 - parse tree/parser

    $ fbt .

resulting in:

    OK - no parse errors in 281 datafile(s)


### step 3 - name (error) checks and more

only check leagues (turn off name check for teams)

    $ fbchk . --no-teams

the full monty

    $ fbchk .

resulting in:

```
!! 269 NAME ERRORS in 281 datafile(s)
[["2001-02/ar.1.txt", "NAME ERROR - no team match found for >Colón de Santa Fe<"],
 ["2001-02/ar.1.txt", "NAME ERROR - no team match found for >Gimnasia de La Plata<"],
 ["2001-02/ar.1.txt", "NAME ERROR - no team match found for >Colón de Santa Fe<"],
 ["2001-02/ar.1.txt", "NAME ERROR - no team match found for >Gimnasia de La Plata<"],
 ["2004-05/eng.4.txt", "NAME ERROR - no team match found for >Chester City<"],
 ["2005-06/eng.4.txt", "NAME ERROR - no team match found for >Chester City<"],
 ["2006-07/eng.4.txt", "NAME ERROR - no team match found for >Chester City<"],
 ["2007-08/eng.4.txt", "NAME ERROR - no team match found for >Chester City<"],
 ["2008-09/eng.4.txt", "NAME ERROR - no team match found for >Chester City<"],
 ["2016-17/eng.5.txt", "NAME ERROR - no team match found for >North Ferriby United<"],
 ["2020-21/at.2.txt", "NAME ERROR - no team match found for >Austria Wien II<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >Sassari Latte Dolce<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >SSD Città di Teramo<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >Casarano<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >US Alessandria 1912<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >Gelbison<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >US Pontedera<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >US Arezzo<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >GSD Ambrosiana<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >Aurora Pro Patria<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >Virtus Francavilla<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >ASD Trastevere<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >SS Tritium 1908<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >ASD Pineto Calcio<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >US Triestina<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >US Breno<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >SS Monopoli 1966<"],
 ["2020-21/it.cup.txt", "NAME ERROR - no team match found for >SN Notaresco<"],
 ["2021-22/it.2.txt", "NAME ERROR - no team match found for >L.R. Vicenza<"],
 ["2021-22/it.2.txt", "NAME ERROR - no team match found for >US Alessandria 1912<"],
 ["2021-22/it.2.txt", "NAME ERROR - no team match found for >L.R. Vicenza<"],
 ["2021-22/it.cup.txt", "NAME ERROR - no team match found for >US Alessandria 1912<"],
 ["2021-22/it.cup.txt", "NAME ERROR - no team match found for >L.R. Vicenza<"],
 ["2023/by.1.txt", "NAME ERROR - no team match found for >FK Minsk<"],
 ["2023/by.1.txt", "NAME ERROR - no team match found for >FK Isloch Minsk<"],
 ["2023/by.1.txt", "NAME ERROR - no team match found for >Torpedo-BelAZ Zhodino<"],
 ["2023/by.1.txt", "NAME ERROR - no team match found for >Naftan Novopolotsk<"],
 ["2023/by.1.txt", "NAME ERROR - no team match found for >Energetik-BGU Minsk<"],
 ["2023/by.1.txt", "NAME ERROR - no team match found for >FK Slutsk<"],
 ["2023/ee.1.txt", "NAME ERROR - no team match found for >Harju JK<"],
 ["2023/ee.1.txt", "NAME ERROR - no team match found for >JK Tammeka<"],
 ["2023/ge.1.txt", "NAME ERROR - no team match found for >Shukura Kobuleti<"],
 ["2023/ge.1.txt", "NAME ERROR - no team match found for >Samgurali Tskhaltubo<"],
 ["2023/kz.1.txt", "NAME ERROR - no team match found for >Zhetysu Taldykorgan<"],
 ["2023/kz.1.txt", "NAME ERROR - no team match found for >FK Aksu<"],
 ["2023/kz.1.txt", "NAME ERROR - no team match found for >FK Ordabasy<"],
 ["2023/kz.1.txt", "NAME ERROR - no team match found for >Kaspiy Aktau<"],
 ["2023/kz.1.txt", "NAME ERROR - no team match found for >FK Atyrau<"],
 ["2023/kz.1.txt", "NAME ERROR - no team match found for >Kaysar Kyzylorda<"],
 ["2023/kz.1.txt", "NAME ERROR - no team match found for >FK Kyzylzhar<"],
 ["2023/kz.1.txt", "NAME ERROR - no team match found for >FK Makhtaaral<"],
 ["2023/kz.1.txt", "NAME ERROR - no team match found for >FK Okzhetpes<"],
 ["2023/lv.1.txt", "NAME ERROR - no team match found for >SK Super Nova<"],
 ["2023/lv.1.txt", "NAME ERROR - no team match found for >FK Metta<"],
 ["2023-24/ad.1.txt", "NAME ERROR - no team match found for >CF Atlètic Amèrica<"],
 ["2023-24/al.1.txt", "NAME ERROR - no team match found for >Egnatia Rrogozhine<"],
 ["2023-24/al.1.txt", "NAME ERROR - no team match found for >Erzeni Shijak<"],
 ["2023-24/al.1.txt", "NAME ERROR - no team match found for >Egnatia Rrogozhine<"],
 ["2023-24/am.1.txt", "NAME ERROR - no team match found for >FK Van<"],
 ["2023-24/am.1.txt", "NAME ERROR - no team match found for >FC West Armenia<"],
 ["2023-24/am.1.txt", "NAME ERROR - no team match found for >BKMA Yerevan<"],
 ["2023-24/ba.1.txt", "NAME ERROR - no team match found for >Zvijezda 09 Bijeljina<"],
 ["2023-24/ba.1.txt", "NAME ERROR - no team match found for >Sloga Doboj<"],
 ["2023-24/ba.1.txt", "NAME ERROR - no team match found for >HŠK Posušje<"],
 ["2023-24/ba.1.txt", "NAME ERROR - no team match found for >Igman Konjic<"],
 ["2023-24/bg.1.txt", "NAME ERROR - no team match found for >Arda Kardzhali<"],
 ["2023-24/bg.1.txt", "NAME ERROR - no team match found for >Arda Kardzhali<"],
 ["2023-24/cy.1.txt", "NAME ERROR - no team match found for >Paphos FC<"],
 ["2023-24/cy.1.txt", "NAME ERROR - no team match found for >AE Zakakiou<"],
 ["2023-24/cy.1.txt", "NAME ERROR - no team match found for >Nea Salamina<"],
 ["2023-24/cy.1.txt", "NAME ERROR - no team match found for >Nea Salamina<"],
 ["2023-24/cy.1.txt", "NAME ERROR - no team match found for >AE Zakakiou<"],
 ["2023-24/cy.1.txt", "NAME ERROR - no team match found for >Paphos FC<"],
 ["2023-24/gr.1.txt", "NAME ERROR - no team match found for >Olympiakos Piraeus<"],
 ["2023-24/gr.1.txt", "NAME ERROR - no team match found for >AE Kifisias<"],
 ["2023-24/gr.1.txt", "NAME ERROR - no team match found for >Olympiakos Piraeus<"],
 ["2023-24/gr.1.txt", "NAME ERROR - no team match found for >AE Kifisias<"],
 ["2023-24/it.3.a.txt", "NAME ERROR - no team match found for >Aurora Pro Patria<"],
 ["2023-24/it.3.a.txt", "NAME ERROR - no team match found for >FC Legnago Salus<"],
 ["2023-24/it.3.a.txt", "NAME ERROR - no team match found for >Arzignano Valchiampo<"],
 ["2023-24/it.3.a.txt", "NAME ERROR - no team match found for >Atalanta II<"],
 ["2023-24/it.3.a.txt", "NAME ERROR - no team match found for >Virtus Verona<"],
 ["2023-24/it.3.a.txt", "NAME ERROR - no team match found for >FC Lumezzane<"],
 ["2023-24/it.3.a.txt", "NAME ERROR - no team match found for >L.R. Vicenza<"],
 ["2023-24/it.3.a.txt", "NAME ERROR - no team match found for >US Alessandria 1912<"],
 ["2023-24/it.3.a.txt", "NAME ERROR - no team match found for >US Fiorenzuola<"],
 ["2023-24/it.3.a.txt", "NAME ERROR - no team match found for >US Pergolettese<"],
 ["2023-24/it.3.a.txt", "NAME ERROR - no team match found for >AC Pro Sesto<"],
 ["2023-24/it.3.a.txt", "NAME ERROR - no team match found for >US Triestina<"],
 ["2023-24/it.3.a.txt", "NAME ERROR - no team match found for >Trento Calcio 1921<"],
 ["2023-24/it.3.a.txt", "NAME ERROR - no team match found for >US Fiorenzuola<"],
 ["2023-24/it.3.b.txt", "NAME ERROR - no team match found for >AC Rimini<"],
 ["2023-24/it.3.b.txt", "NAME ERROR - no team match found for >US Arezzo<"],
 ["2023-24/it.3.b.txt", "NAME ERROR - no team match found for >ASD Pineto Calcio<"],
 ["2023-24/it.3.b.txt", "NAME ERROR - no team match found for >US Pontedera<"],
 ["2023-24/it.3.b.txt", "NAME ERROR - no team match found for >USD Sestri Levante<"],
 ["2023-24/it.3.b.txt", "NAME ERROR - no team match found for >US Recanatese<"],
 ["2023-24/it.3.b.txt", "NAME ERROR - no team match found for >SEF Torres 1903<"],
 ["2023-24/it.3.b.txt", "NAME ERROR - no team match found for >Vis Pesaro<"],
 ["2023-24/it.3.b.txt", "NAME ERROR - no team match found for >Ancona 1905<"],
 ["2023-24/it.3.b.txt", "NAME ERROR - no team match found for >Juventus II<"],
 ["2023-24/it.3.b.txt", "NAME ERROR - no team match found for >Olbia Calcio<"],
 ["2023-24/it.3.b.txt", "NAME ERROR - no team match found for >US Recanatese<"],
 ["2023-24/it.3.b.txt", "NAME ERROR - no team match found for >Vis Pesaro<"],
 ["2023-24/it.3.c.txt", "NAME ERROR - no team match found for >Giugliano<"],
 ["2023-24/it.3.c.txt", "NAME ERROR - no team match found for >Sorrento Calcio<"],
 ["2023-24/it.3.c.txt", "NAME ERROR - no team match found for >Audace Cerignola<"],
 ["2023-24/it.3.c.txt", "NAME ERROR - no team match found for >Monterosi FC<"],
 ["2023-24/it.3.c.txt", "NAME ERROR - no team match found for >Brindisi<"],
 ["2023-24/it.3.c.txt", "NAME ERROR - no team match found for >Taranto FC<"],
 ["2023-24/it.3.c.txt", "NAME ERROR - no team match found for >FC Turris<"],
 ["2023-24/it.3.c.txt", "NAME ERROR - no team match found for >Virtus Francavilla<"],
 ["2023-24/it.3.c.txt", "NAME ERROR - no team match found for >AZ Picerno<"],
 ["2023-24/it.3.c.txt", "NAME ERROR - no team match found for >SS Monopoli 1966<"],
 ["2023-24/it.3.c.txt", "NAME ERROR - no team match found for >Casertana FC<"],
 ["2023-24/it.3.c.txt", "NAME ERROR - no team match found for >Virtus Francavilla<"],
 ["2023-24/it.3.c.txt", "NAME ERROR - no team match found for >SS Monopoli 1966<"],
 ["2023-24/it.3.c.txt", "NAME ERROR - no team match found for >Monterosi FC<"],
 ["2023-24/it.cup.txt", "NAME ERROR - no team match found for >L.R. Vicenza<"],
 ["2023-24/kos.1.txt", "NAME ERROR - no team match found for >KF Liria<"],
 ["2023-24/kos.1.txt", "NAME ERROR - no team match found for >KF Ballkani<"],
 ["2023-24/kos.1.txt", "NAME ERROR - no team match found for >KF Fushë Kosova<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >FC Triesen III<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >FC Vaduz III<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >FC Schaan<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >USV Eschen/Mauren II<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >FC Triesen<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >FC Triesen II<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >FC Triesenberg<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >FC Ruggell<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >FC Schaan II<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >FC Triesenberg II<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >FC Vaduz II<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >FC Balzers<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >FC Ruggell II<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >FC Balzers II<"],
 ["2023-24/li.cup.txt", "NAME ERROR - no team match found for >USV Eschen/Mauren III<"],
 ["2023-24/lu.1.txt", "NAME ERROR - no team match found for >FC Schifflange 95<"],
 ["2023-24/lu.1.txt", "NAME ERROR - no team match found for >UN Käerjéng<"],
 ["2023-24/lu.1.txt", "NAME ERROR - no team match found for >Marisca Mersch<"],
 ["2023-24/md.1.txt", "NAME ERROR - no team match found for >FC Bălţi<"],
 ["2023-24/md.1.txt", "NAME ERROR - no team match found for >Sparta Selemet<"],
 ["2023-24/md.1.txt", "NAME ERROR - no team match found for >FC Bălţi<"],
 ["2023-24/me.1.txt", "NAME ERROR - no team match found for >Jedinstvo Bijelo Polje<"],
 ["2023-24/me.1.txt", "NAME ERROR - no team match found for >OFK Mladost DG<"],
 ["2023-24/me.1.txt", "NAME ERROR - no team match found for >FK Arsenal<"],
 ["2023-24/mk.1.txt", "NAME ERROR - no team match found for >FK Bregalnica Štip<"],
 ["2023-24/mt.1.txt", "NAME ERROR - no team match found for >St. Luċija FC<"],
 ["2023-24/nir.1.txt", "NAME ERROR - no team match found for >Newry City FC<"],
 ["2023-24/rs.1.txt", "NAME ERROR - no team match found for >IMT Beograd<"],
 ["2023-24/rs.1.txt", "NAME ERROR - no team match found for >Železničar Pančevo<"],
 ["2023-24/rs.1.txt", "NAME ERROR - no team match found for >IMT Beograd<"],
 ["2023-24/rs.1.txt", "NAME ERROR - no team match found for >Železničar Pančevo<"],
 ["2023-24/sk.1.txt", "NAME ERROR - no team match found for >FC DAC 1904<"],
 ["2023-24/sk.1.txt", "NAME ERROR - no team match found for >FC DAC 1904<"],
 ["2023-24/ua.1.txt", "NAME ERROR - no team match found for >NK Veres<"],
 ["2023-24/ua.1.txt", "NAME ERROR - no team match found for >FK Obolon<"],
 ["2023-24/ua.1.txt", "NAME ERROR - no team match found for >FK Oleksandriya<"],
 ["2023-24/wal.1.txt", "NAME ERROR - no team match found for >Pontypridd United<"],
 ["2023-24/wal.1.txt", "NAME ERROR - no team match found for >Colwyn Bay FC<"],
 ["2023-24/wal.1.txt", "NAME ERROR - no team match found for >Colwyn Bay FC<"],
 ["2023-24/wal.1.txt", "NAME ERROR - no team match found for >Pontypridd United<"],
 ["2024/by.1.txt", "NAME ERROR - no team match found for >FK Isloch Minsk<"],
 ["2024/by.1.txt", "NAME ERROR - no team match found for >Naftan Novopolotsk<"],
 ["2024/by.1.txt", "NAME ERROR - no team match found for >FK Minsk<"],
 ["2024/by.1.txt", "NAME ERROR - no team match found for >Torpedo-BelAZ Zhodino<"],
 ["2024/by.1.txt", "NAME ERROR - no team match found for >FK Slutsk<"],
 ["2024/ee.1.txt", "NAME ERROR - no team match found for >JK Tammeka<"],
 ["2024/ge.1.txt", "NAME ERROR - no team match found for >Kolkheti Poti<"],
 ["2024/ge.1.txt", "NAME ERROR - no team match found for >Samgurali Tskhaltubo<"],
 ["2024/kz.1.txt", "NAME ERROR - no team match found for >Kaysar Kyzylorda<"],
 ["2024/kz.1.txt", "NAME ERROR - no team match found for >FK Zhenis<"],
 ["2024/kz.1.txt", "NAME ERROR - no team match found for >FK Yelimay<"],
 ["2024/kz.1.txt", "NAME ERROR - no team match found for >FK Atyrau<"],
 ["2024/kz.1.txt", "NAME ERROR - no team match found for >FK Ordabasy<"],
 ["2024/kz.1.txt", "NAME ERROR - no team match found for >FK Turan<"],
 ["2024/kz.1.txt", "NAME ERROR - no team match found for >FK Kyzylzhar<"],
 ["2024/kz.1.txt", "NAME ERROR - no team match found for >Zhetysu Taldykorgan<"],
 ["2024/lv.1.txt", "NAME ERROR - no team match found for >FK Metta<"],
 ["2024-25/al.1.txt", "NAME ERROR - no team match found for >Egnatia Rrogozhine<"],
 ["2024-25/al.1.txt", "NAME ERROR - no team match found for >KF Bylis Ballsh<"],
 ["2024-25/am.1.txt", "NAME ERROR - no team match found for >BKMA Yerevan<"],
 ["2024-25/am.1.txt", "NAME ERROR - no team match found for >FK Van<"],
 ["2024-25/am.1.txt", "NAME ERROR - no team match found for >FC West Armenia<"],
 ["2024-25/at.3.o.txt", "NAME ERROR - no team match found for >Austria Wien II<"],
 ["2024-25/az.1.txt", "NAME ERROR - no team match found for >Şamaxı FK<"],
 ["2024-25/ba.1.txt", "NAME ERROR - no team match found for >HŠK Posušje<"],
 ["2024-25/ba.1.txt", "NAME ERROR - no team match found for >Igman Konjic<"],
 ["2024-25/ba.1.txt", "NAME ERROR - no team match found for >Sloga Doboj<"],
 ["2024-25/bg.1.txt", "NAME ERROR - no team match found for >Arda Kardzhali<"],
 ["2024-25/bg.1.txt", "NAME ERROR - no team match found for >Septemvri Sofia<"],
 ["2024-25/ch.cup.txt", "NAME ERROR - no team match found for >Lancy FC<"],
 ["2024-25/ch.cup.txt", "NAME ERROR - no team match found for >FC Besa St. Gallen<"],
 ["2024-25/ch.cup.txt", "NAME ERROR - no team match found for >Signal FC Bernex-Confignon<"],
 ["2024-25/cy.1.txt", "NAME ERROR - no team match found for >Omonia 29is Maiou<"],
 ["2024-25/cy.1.txt", "NAME ERROR - no team match found for >Paphos FC<"],
 ["2024-25/cy.1.txt", "NAME ERROR - no team match found for >Nea Salamina<"],
 ["2024-25/gr.1.txt", "NAME ERROR - no team match found for >Olympiakos Piraeus<"],
 ["2024-25/gr.1.txt", "NAME ERROR - no team match found for >GS Kallithea<"],
 ["2024-25/it.3.a.txt", "NAME ERROR - no team match found for >Atalanta II<"],
 ["2024-25/it.3.a.txt", "NAME ERROR - no team match found for >ASC Alcione<"],
 ["2024-25/it.3.a.txt", "NAME ERROR - no team match found for >US Triestina<"],
 ["2024-25/it.3.a.txt", "NAME ERROR - no team match found for >Arzignano Valchiampo<"],
 ["2024-25/it.3.a.txt", "NAME ERROR - no team match found for >Caldiero Terme<"],
 ["2024-25/it.3.a.txt", "NAME ERROR - no team match found for >Clodiense SSD<"],
 ["2024-25/it.3.a.txt", "NAME ERROR - no team match found for >Aurora Pro Patria<"],
 ["2024-25/it.3.a.txt", "NAME ERROR - no team match found for >Virtus Verona<"],
 ["2024-25/it.3.a.txt", "NAME ERROR - no team match found for >FC Lumezzane<"],
 ["2024-25/it.3.a.txt", "NAME ERROR - no team match found for >L.R. Vicenza<"],
 ["2024-25/it.3.a.txt", "NAME ERROR - no team match found for >US Pergolettese<"],
 ["2024-25/it.3.a.txt", "NAME ERROR - no team match found for >Trento Calcio 1921<"],
 ["2024-25/it.3.b.txt", "NAME ERROR - no team match found for >ASD Pineto Calcio<"],
 ["2024-25/it.3.b.txt", "NAME ERROR - no team match found for >US Pianese<"],
 ["2024-25/it.3.b.txt", "NAME ERROR - no team match found for >FC Legnago Salus<"],
 ["2024-25/it.3.b.txt", "NAME ERROR - no team match found for >US Pontedera<"],
 ["2024-25/it.3.b.txt", "NAME ERROR - no team match found for >USD Sestri Levante<"],
 ["2024-25/it.3.b.txt", "NAME ERROR - no team match found for >US Arezzo<"],
 ["2024-25/it.3.b.txt", "NAME ERROR - no team match found for >Campobasso<"],
 ["2024-25/it.3.b.txt", "NAME ERROR - no team match found for >AC Milan II<"],
 ["2024-25/it.3.b.txt", "NAME ERROR - no team match found for >SEF Torres 1903<"],
 ["2024-25/it.3.b.txt", "NAME ERROR - no team match found for >Vis Pesaro<"],
 ["2024-25/it.3.b.txt", "NAME ERROR - no team match found for >AC Carpi<"],
 ["2024-25/it.3.b.txt", "NAME ERROR - no team match found for >AC Rimini<"],
 ["2024-25/it.3.c.txt", "NAME ERROR - no team match found for >Juventus II<"],
 ["2024-25/it.3.c.txt", "NAME ERROR - no team match found for >Audace Cerignola<"],
 ["2024-25/it.3.c.txt", "NAME ERROR - no team match found for >Casertana FC<"],
 ["2024-25/it.3.c.txt", "NAME ERROR - no team match found for >Giugliano<"],
 ["2024-25/it.3.c.txt", "NAME ERROR - no team match found for >Taranto FC<"],
 ["2024-25/it.3.c.txt", "NAME ERROR - no team match found for >Sorrento Calcio<"],
 ["2024-25/it.3.c.txt", "NAME ERROR - no team match found for >AZ Picerno<"],
 ["2024-25/it.3.c.txt", "NAME ERROR - no team match found for >FC Turris<"],
 ["2024-25/it.3.c.txt", "NAME ERROR - no team match found for >SS Monopoli 1966<"],
 ["2024-25/it.3.c.txt", "NAME ERROR - no team match found for >Cavese<"],
 ["2024-25/it.3.c.txt", "NAME ERROR - no team match found for >Team Altamura<"],
 ["2024-25/it.cup.txt", "NAME ERROR - no team match found for >SEF Torres 1903<"],
 ["2024-25/it.cup.txt", "NAME ERROR - no team match found for >N.N.<"],
 ["2024-25/kos.1.txt", "NAME ERROR - no team match found for >KF Ballkani<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >FC Balzers III<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >FC Vaduz III<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >FC Ruggell II<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >FC Schaan<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >FC Ruggell<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >FC Triesen<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >USV Eschen/Mauren II<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >FC Schaan II<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >FC Balzers II<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >FC Vaduz II<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >FC Triesenberg II<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >FC Triesen II<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >USV Eschen/Mauren III<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >FC Balzers<"],
 ["2024-25/li.cup.txt", "NAME ERROR - no team match found for >FC Triesenberg<"],
 ["2024-25/md.1.txt", "NAME ERROR - no team match found for >Sparta Selemet<"],
 ["2024-25/md.1.txt", "NAME ERROR - no team match found for >FC Bălţi<"],
 ["2024-25/me.1.txt", "NAME ERROR - no team match found for >FK Arsenal<"],
 ["2024-25/me.1.txt", "NAME ERROR - no team match found for >Jedinstvo Bijelo Polje<"],
 ["2024-25/me.1.txt", "NAME ERROR - no team match found for >FK Otrant Ulcinj<"],
 ["2024-25/mt.1.txt", "NAME ERROR - no team match found for >St. Patrick FC<"],
 ["2024-25/ro.1.txt", "NAME ERROR - no team match found for >Gloria Buzău<"],
 ["2024-25/rs.1.txt", "NAME ERROR - no team match found for >Železničar Pančevo<"],
 ["2024-25/rs.1.txt", "NAME ERROR - no team match found for >IMT Beograd<"],
 ["2024-25/ru.1.txt", "NAME ERROR - no team match found for >Akron Tolyatti<"],
 ["2024-25/ru.1.txt", "NAME ERROR - no team match found for >FK Dinamo Makhachkala<"],
 ["2024-25/sk.1.txt", "NAME ERROR - no team match found for >FC DAC 1904<"],
 ["2024-25/ua.1.txt", "NAME ERROR - no team match found for >NK Veres<"],
 ["2024-25/ua.1.txt", "NAME ERROR - no team match found for >FK Oleksandriya<"],
 ["2024-25/ua.1.txt", "NAME ERROR - no team match found for >FK Obolon<"],
 ["2024-25/uefa.cl.txt", "NAME ERROR - no team match found for >AS Monaco (FRA)<"],
 ["2024-25/uefa.cl.txt",
  "PARSE ERROR - country code missing for club name in int'l tournament; may not be unique >N.N.<"]]
```


