Kas ir api?

Api ir lietotnes programmēšanas interfeiss.
Tas strādā kā starpnieks, kas ļauj divām programmām sazināties savā starpā. Tas definē noteikumus un specifikācijas, kā programmas var apmainīties ar datiem un funkcijām.

Mainīgā deklarēšana PHP

PHP valodā mainīgos var deklarēt, izmantojot $ simbolu un mainīgā nosaukumu. 
Mainīgā nosaukumam jāuzsākas ar burtu vai apakšsvītru (_), un tam var sekot burti, cipari un apakšsvītras.
Piemēram, $vards = "Kristiāns";

Kādu arhitektūru izmanto Laravel, paskaidro kā tā strādā

Laravel ir PHP ietvaru sistēma, kas balstīta uz Model-View-Controller arhitektūru. Šī arhitektūra sadala lietojumprogrammu trīs slāņos:

Modelis: Šajā slānī tiek definēti lietojumprogrammas dati un biznesa loģika.

Skats: Šajā slānī tiek definēta lietojumprogrammas lietotāja saskarne.

Kontrolētājs: Šajā slānī tiek apstrādāta lietotāja mijiedarbība un tiek sūtīti pieprasījumi modelim un skatam.

Laravel arhitektūra ir modulāra un ļauj viegli izveidot sarežģītas tīmekļa lietojumprogrammas.


Kas ir ORM, kāpēc to izmanto tīra SQL vietā?

ORM ir programmēšanas tehnika, kas pārveido datus no relatīvajām datu bāzēm (izmantojot SQL) uz objektorientētām programmēšanas valodām (tādām kā PHP, Java, Python u.c.). 
Ar ORM datu bāzes tabulas tiek attēlotas kā klases, bet datu bāzes ieraksti - kā klases objekti.

ORM ļauj strādāt ar datubāzes datiem, izmantojot objektus savā programmēšanas valodā .
Tas nozīmē, ka nav tieši jāraksta SQL vaicājumi. Datu bāzes tabulas tiek pārvērstas klasēs, bet ieraksti - objektos.
Kāpēc izmantot ORM tīra SQL vietā:

Darbs ar objektiem parasti ir ērtāks izstrādātājiem nekā ar tīru SQL.
ORM var paātrināt izstrādi, jo nav jāraksta sarežģīti SQL vaicājumi.
ORM palīdz uzturēt tīrāku un labāk organizētu kodu.
ORM ietvari bieži ietver iebūvētus drošības līdzekļus, piemēram, aizsardzību pret SQL injekcijām.

Uzraksti Eloquent ORM pieprasījumu modelim User, kur nepieciešams iegūt visus
lietotājus kuriem reitings ir lielāks par 4. 

$users = User::where('rating', '>', 4)->get();