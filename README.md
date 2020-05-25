# Zwicker

The dataset contains training and test data used to verify the authorship of the anti-heretical treatise Refutatio errorum. 

Dataset authors:

Reima Välimäki: data selection, analysis and description

Aleksi Vesanto: data pre-processing and analysis

Anni Hella: data pre-processing


Publications:
Reima Välimäki, Aleksi Vesanto, Anni Hella, Adam Poznański, Filip Ginter: ”Manuscripts,
qualitative analysis and features on vectors. An attempt for a synthesis of conventional and
computational methods in the attribution of late medieval anti-heretical treatises”. Petri Paju, Mila Oiva & Mats Fridlund (eds.) Digital, Computational and Distant Readings of History: Emergent approaches within the new digital history. Helsinki: Helsinki University Press 2020 (forthcoming)

Description of the data:

The dataset has two gzip files containing the Latin text data used to train the SVM classifier. In addition, there is a wordlist of 1000 most common latin words (gzip and json files) used in text distortion (masking).

The data is shared in masked form only to protect copyrights of recent editions used in the corpus

The texts included in the data are:

TEST DATA: (test_data_september_mask.gz)

TEST1: Refutatio errorum, Redaction 4a; Source: Augsburg, Staats- und Stadtbibliothek, MS 338, fols. 159r–170r.

TEST2: Refutatio errorum, Redaction 4b; Source: Gretser, J. (Ed.). (1677). Lucae Tvdensis episcopi, Scriptores aliqvot svccedanei contra sectam waldensivm. Maxima Bibliotheca Veterum Patrum, Et Antiquorum Scriptorum Ecclesiasticorum. Tom. XXV. Lvgdvni: Anissonios, 302G–307F.

TEST3: Refutatio errorum, Redaction 1; Source: Vienna, Österreichische Nationalbibliothek, MS 1588, fols. 191r–211v.

TRAINING DATA (train_data_september_mask.gz)

Suspected author: Petrus Zwicker: Text: Cum dormirent homines (CDH); Source: Gretser, J. (Ed.). (1677). Lucae Tvdensis episcopi, Scriptores aliqvot svccedanei contra sectam waldensivm. Maxima Bibliotheca Veterum Patrum, Et Antiquorum Scriptorum Ecclesiasticorum. Tom. XXV. Lvgdvni: Anissonios, 277F–299G.

Other authors:

Author: Alanus de Insulis (Alain of Lille); Text: Contra haereticos; Source: Patrologia Latina 210. Text from Corpus Corporum: http://mlat.uzh.ch/?c=2&w=AlDeIn.ConHae

Author: Anonymous; Text: Attendite a falsis prophetis; Source: St. Florian, MS XI 152, fols. 48v–50v.

Author: Anonymous; Text: Disputatio inter Catholicum et Paterinum hereticum; Source: Hoécker, C. (Ed.). (2001). Disputatio inter catholicum et paterinum hereticum: die Auseinandersetzung der katholischen Kirche mit den italienischen Katharern im Spiegel einer kontroverstheologischen Streitschrift des 13. Jahrhunderts. Tavarnuzze (Firenze): SISMEL edizioni del Galluzzo, 3–80.

Author: Anonymous of Passau; Text: Tractatus de erroribus hereticorum; Source: Nickson, M. A. E. (1962). A critical edition of the treatise on heresy ascribed to Pseudo-Reinerius, with an historical introduction. Queen Mary, University of London, 1–154.

Author: Augustinus of Hippo; Text: Contra Faustum Manichaeum; Source: Patrologia Latina 42. Text from Corpus Corporum: http://mlat.uzh.ch/?c=2&w=AugHip.CoFaMa

Author: Augustinus of Hippo; Text: Contra epistulam Fundamenti; Source: Corpus Scriptorum Ecclesiasticorum Latinorum (CSEL) 25.1. Text from Corpus corporum: 
http://mlat.uzh.ch/?c=19&w=August.CoEpFunCSEL

Author: Berthold von Regensburg; Text: Sermones [XXIIII, XXVIII, XXVIIII, ‘Sancti pre Fidem’ and ‘Dominica Duodecima’]; Source: Czerwon, A. (2011). Predigt gegen Ketzer: Studien zu den lateinischen Sermones Bertholds von Regensburg. Tübingen: Mohr Siebeck, 203–233.

Author: Durand of Huesca; Text: Liber contra manicheos; Source: Thouzellier, C. (1964). Une somme anti-cathare: le Liber contra Manicheos de Durand de Huesca. Louvain: Spicilegium sacrum Lovaniense, 67–336.

Author: Durand of Huesca; Text: Liber Antiheresis; Source: Selge, K.-V. (Ed.) (1967). Die ersten Waldenser: mit Edition des Liber antiheresis des Durandus von Osca (Vol. 2). Berlin: De Gruyter, 3–257.

Author: Hermannus of Scildis; Text: Tractatus contra haereticos; Source: Zumkeller, A. (1970). Hermanni de Scildis O.S.A.: tractatus contra haereticos negantes immunitatem et iurisdictionem sanctae Ecclesiae et Tractatus de conceptione gloriosae virginis Mariae. Würzburg: Augustinus-Verl., 3–108. 

Author: Johannes Cassianus; Text: De incarnatione Domini contra Nestorium; Source: Corpus Scriptorum Ecclesiasticorum Latinorum (CSEL) 17. Text from Corpus Corporum: http://mlat.uzh.ch/?c=19&w=Cassia.ConNesCSEL

Author: Moneta Cremonensis (Moneta of Cremona); Text: Adversus Catharos et Valdenses, Liber V; Source: Moneta (Cremonensis). (1743). Monetae Adversus Catharos et Valdenses: libri quinque. T. A. Ricchini (Ed.). Romae: Ex Typographia Palladis, 389–560.

Author: Petrus de Pillichsdorf (Peter von Pillichsdorf); Text: Contra Pauperes de Lugduno; Source: Gretser, J. (Ed.) (1677). Lucae Tvdensis episcopi, Scriptores aliqvot svccedanei contra sectam waldensivm. Maxima Bibliotheca Veterum Patrum, Et Antiquorum Scriptorum Ecclesiasticorum. Tom. XXV. Lvgdvni: Anissonios, 299E–302F.

Author: Petrus Veronensis (?); Text: Summa contra haereticos; Source: Kaeppeli, T. (1947). Une somme contre les hérétiques de S. Pierre Martyr (?). Archivum Fratrum Praedicatorum, 17, 295–335

Author: Wasmud von Homburg; Text: Tractatus contra hereticos Beckardos, Lulhardos et Swestriones; Source: Schmidt, A. (Ed.) (1962). Tractatus contra hereticos Beckardos, Lulhardos et Swestriones des Wasmud von Homburg. Archiv für mittelrheinische Kirchengeschichte, 14, 336–386.


Data preprocessing:
Normalization rules to solve ortographical variation:
u-> v
j -> i
y -> i
ae -> e
oe -> e
char->car (to solve variation charitas vs. caritas)
wa -> va (to solve variation ewangelium / evangelium and waldenses / valdenses)

These solve the majority of orthographical variation caused by editorial and scribal conventions and the differences of medieval and classical Latin without masking potentially significant stylistic features. In addition to orthographical normalisation, in the pre-processing phase we cleaned the texts from editorial additions such as page numbers and chapter titles (unless part of the original). Punctuation, numerals and single characters were removed. From early medieval texts we cleaned the references to bible books and verses (which were added by later editors), but in late medieval texts, most notably Zwicker’s own treatise, these are part of the original and were thus preserved. The pre-processing was done automatically, but confirmed with sanity checks. 

Texts were masked using a list of the thousand most common word forms in post-classical (Christian) Latin, based on a corpus of 15 million words. Any word not in the calculated word list was be masked with a series of X-signs corresponding the length of the word. 


Related code:
https://github.com/avjves/AuthAttHelper

File formats:
txt, gzip, json

 
