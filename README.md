# Estudi exploratori sobre la robustesa dialectal dels LLMs en català

### Visió general

Aquest projecte presenta un estudi exploratori sobre la capacitat dels models grans de llenguatge per entendre i generar varietats dialectals del català. L’objectiu és analitzar fins a quin punt els LLMs actuals preserven la riquesa dialectal de la llengua o tendeixen a normalitzar les respostes cap a formes més estàndard, centrals o majoritàries.

El treball va ser desenvolupat en el marc de l’assignatura **Models Grans de Llenguatge (MGL)** del **Grau en Intel·ligència Artificial** a la **Universitat Politècnica de Catalunya (UPC)**.

---

### Objectiu

L’estudi se centra en el possible **biaix d’estandardització** dels models generatius en català. Aquest biaix apareix quan un model, davant d’una varietat dialectal concreta, genera formes massa generals, centrals o normatives, deixant de banda trets lingüístics propis d’altres zones catalanoparlants.

El projecte avalua si els models són capaços de mantenir la variació dialectal en tasques relacionades amb morfologia, lèxic, fraseologia i registre informal.

---

### Models avaluats

L’estudi compara respostes generades per tres models d’última generació mitjançant Arena AI:

| Model | Plataforma d'avaluació | Tipus d'avaluació |
| :--- | :--- | :--- |
| GPT-5.2-chat | Arena AI | Comparació manual |
| Claude 4.6 | Arena AI | Comparació manual |
| Gemini 3-Flash | Arena AI | Comparació manual |

---

### Metodologia i components

El procés d’avaluació es basa en una bateria de prompts dissenyats manualment per posar a prova la competència dialectal dels models.

| Etapa | Tècnica principal | Finalitat |
| :--- | :--- | :--- |
| Disseny de prompts | Stress tests lingüístics | Avaluar fenòmens dialectals específics |
| Generació de respostes | Arena AI | Comparar models sota condicions equivalents |
| Avaluació manual | Rúbrica ponderada | Mesurar qualitat lingüística i adequació dialectal |
| Anàlisi qualitativa | Comentari lingüístic | Identificar errors, patrons i biaixos |

---

### Criteris d’avaluació

Les respostes dels models s’avaluen segons tres dimensions:

- **Gramaticalitat (GR):** correcció morfològica, sintàctica i ortogràfica.
- **Adequació dialectal (AD):** coherència amb la varietat dialectal sol·licitada.
- **Fidelitat a la tasca (FT):** compliment del prompt i de les instruccions.

La puntuació ponderada de cada experiment es calcula com:

$$
Score_i = 0.4 \cdot GR + 0.4 \cdot AD + 0.2 \cdot FT
$$

La puntuació final de cada model correspon a la mitjana dels resultats obtinguts en tots els experiments.

---

### Experiments

L’estudi inclou sis experiments centrats en diferents fenòmens de variació dialectal catalana:

| Experiment | Varietat o fenomen | Objectiu |
| :--- | :--- | :--- |
| 1 | Morfologia verbal valenciana | Avaluar formes verbals en present d’indicatiu |
| 2 | Mallorquí | Analitzar article salat, pronoms i lèxic balear |
| 3 | Pallarès | Comprovar coneixement de lèxic local |
| 4 | Fraseologia dels Països Catalans | Identificar significat i origen d’expressions |
| 5 | Alguerès i variació geogràfica | Comparar formes lèxiques entre territoris |
| 6 | Menorquí informal | Generar una conversa natural en registre col·loquial |

---

### Resultats principals

Els resultats mostren que els models actuals poden adaptar-se parcialment a varietats dialectals del català, especialment quan els trets són visibles, freqüents o ben documentats. GPT-5.2-chat i Gemini 3-Flash obtenen els millors resultats globals, mentre que Claude 4.6 presenta un rendiment més irregular en les proves realitzades.

| Model | Puntuació final |
| :--- | ---: |
| GPT-5.2-chat | 8.77 |
| Gemini 3-Flash | 8.47 |
| Claude 4.6 | 5.80 |

L’anàlisi també mostra que els models tenen més dificultats amb el lèxic molt local, la fraseologia i els usos informals regionals. Aquest comportament suggereix que, tot i els avenços dels LLMs en català, encara hi ha marge de millora en la representació de la diversitat dialectal.

---

### Conclusions

L’estudi apunta que els LLMs més avançats són capaços de reconèixer i produir determinades formes dialectals catalanes, però el seu coneixement no és homogeni entre varietats ni entre tipus de tasca. Les formes més documentades o transparents solen ser tractades amb més encert, mentre que els mots locals, les expressions fraseològiques i els usos col·loquials mostren més errors o neutralitzacions.

Aquests resultats reforcen la importància de desenvolupar recursos lingüístics, dades dialectals i protocols d’avaluació específics per al català. Una IA lingüísticament robusta no només hauria de generar català correcte, sinó també respectar-ne la variació geogràfica i cultural.

---

### Informe

L’informe complet està disponible al repositori:

[LLMs_dialectal_catala.pdf](./LLMs_dialectal_catala.pdf)

---

### Context acadèmic

Jaume Mora Ladària
Models Grans de Llenguatge (MGL)
Grau en Intel·ligència Artificial
Universitat Politècnica de Catalunya (UPC)
