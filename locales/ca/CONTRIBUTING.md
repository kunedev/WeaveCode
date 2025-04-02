# Contribuir a Weavy

Estem entusiasmats que estigueu interessats en contribuir a Weavy. Ja sigui arreglant un error, afegint una funcionalitat o millorant la nostra documentació, cada contribució fa que Weavy sigui més intel·ligent! Per mantenir la nostra comunitat vibrant i acollidora, tots els membres han de complir el nostre [Codi de Conducta](CODE_OF_CONDUCT.md).

## Uniu-vos a la nostra comunitat

Encoratgem fortament a tots els col·laboradors a unir-se a la nostra [comunitat de Discord](https://discord.gg/roocode)! Formar part del nostre servidor de Discord us ajuda a:

- Obtenir ajuda i orientació en temps real sobre les vostres contribucions
- Connectar amb altres col·laboradors i membres de l'equip principal
- Mantenir-vos al dia sobre els desenvolupaments i prioritats del projecte
- Participar en discussions que configuren el futur de Weavy
- Trobar oportunitats de col·laboració amb altres desenvolupadors

## Informar d'errors o problemes

Els informes d'errors ajuden a millorar Weavy per a tothom! Abans de crear un nou informe, si us plau [cerqueu entre els existents](https://github.com/RooVetGit/Roo-Code/issues) per evitar duplicats. Quan estigueu a punt per informar d'un error, dirigiu-vos a la nostra [pàgina d'incidències](https://github.com/RooVetGit/Roo-Code/issues/new/choose) on trobareu una plantilla per ajudar-vos a completar la informació rellevant.

<blockquote class='warning-note'>
     🔐 <b>Important:</b> Si descobriu una vulnerabilitat de seguretat, utilitzeu l'<a href="https://github.com/RooVetGit/Roo-Code/security/advisories/new">eina de seguretat de Github per informar-ne privadament</a>.
</blockquote>

## Decidir en què treballar

Buscant una bona primera contribució? Consulteu les incidències a la secció "Issue [Unassigned]" del nostre [Projecte de Github de Weavy](https://github.com/orgs/RooVetGit/projects/1). Aquestes estan específicament seleccionades per a nous col·laboradors i àrees on ens encantaria rebre ajuda!

També donem la benvinguda a contribucions a la nostra [documentació](https://docs.roocode.com/)! Ja sigui corregint errors tipogràfics, millorant guies existents o creant nou contingut educatiu - ens encantaria construir un repositori de recursos impulsat per la comunitat que ajudi a tothom a aprofitar al màxim Weavy. Podeu fer clic a "Editar aquesta pàgina" a qualsevol pàgina per arribar ràpidament al lloc correcte a Github per editar el fitxer, o podeu anar directament a https://github.com/RooVetGit/Roo-Code-Docs.

Si esteu planejant treballar en una funcionalitat més gran, si us plau creeu primer una [sol·licitud de funcionalitat](https://github.com/RooVetGit/Roo-Code/discussions/categories/feature-requests?discussions_q=is%3Aopen+category%3A%22Feature+Requests%22+sort%3Atop) perquè puguem discutir si s'alinea amb la visió de Weavy. També podeu consultar el nostre [Full de Ruta del Projecte](#full-de-ruta-del-projecte) a continuació per veure si la vostra idea s'ajusta a la nostra direcció estratègica.

## Full de Ruta del Projecte

Weavy té un full de ruta de desenvolupament clar que guia les nostres prioritats i direcció futura. Entendre el nostre full de ruta us pot ajudar a:

- Alinear les vostres contribucions amb els objectius del projecte
- Identificar àrees on la vostra experiència seria més valuosa
- Entendre el context darrere de certes decisions de disseny
- Trobar inspiració per a noves funcionalitats que donin suport a la nostra visió

El nostre full de ruta actual se centra en sis pilars clau:

### Suport de Proveïdors

Aspirem a donar suport a tants proveïdors com sigui possible:

- Suport més versàtil per a "OpenAI Compatible"
- xAI, Microsoft Azure AI, Alibaba Cloud Qwen, IBM Watsonx, Together AI, DeepInfra, Fireworks AI, Cohere, Perplexity AI, FriendliAI, Replicate
- Suport millorat per a Ollama i LM Studio

### Suport de Models

Volem que Roo funcioni tan bé com sigui possible amb tants models com sigui possible, inclosos els models locals:

- Suport de models locals a través de prompts de sistema personalitzats i fluxos de treball
- Avaluacions de rendiment i casos de prova

### Suport de Sistemes

Volem que Roo funcioni bé a l'ordinador de tothom:

- Integració de terminal multiplataforma
- Suport sòlid i consistent per a Mac, Windows i Linux

### Documentació

Volem documentació completa i accessible per a tots els usuaris i col·laboradors:

- Guies d'usuari i tutorials ampliats
- Documentació clara de l'API
- Millor orientació per als col·laboradors
- Recursos de documentació multilingües
- Exemples interactius i mostres de codi

### Estabilitat

Volem reduir significativament el nombre d'errors i augmentar les proves automatitzades:

- Interruptor de registre de depuració
- Botó de còpia "Informació de Màquina/Tasca" per enviar amb sol·licituds d'error/suport

### Internacionalització

Volem que Roo parli l'idioma de tothom:

- 我们希望 Weavy 说每个人的语言
- Queremos que Weavy hable el idioma de todos
- हम चाहते हैं कि Weavy हर किसी की भाषा बोले
- نريد أن يتحدث Weavy لغة الجميع

Donem especialment la benvinguda a contribucions que avancin els nostres objectius del full de ruta. Si esteu treballant en alguna cosa que s'alinea amb aquests pilars, si us plau mencioneu-ho a la descripció del vostre PR.

## Configuració de desenvolupament

1. **Cloneu** el repositori:

```sh
git clone https://github.com/RooVetGit/Roo-Code.git
```

2. **Instal·leu les dependències**:

```sh
npm run install:all
```

3. **Inicieu la vista web (aplicació Vite/React amb HMR)**:

```sh
npm run dev
```

4. **Depuració**:
   Premeu `F5` (o **Execució** → **Inicia la depuració**) a VSCode per obrir una nova sessió amb Weavy carregat.

Els canvis a la vista web apareixeran immediatament. Els canvis a l'extensió principal requeriran reiniciar l'amfitrió de l'extensió.

Alternativament, podeu crear un .vsix i instal·lar-lo directament a VSCode:

```sh
npm run build
```

Apareixerà un fitxer `.vsix` al directori `bin/` que es pot instal·lar amb:

```sh
code --install-extension bin/roo-cline-<version>.vsix
```

## Escriure i enviar codi

Qualsevol persona pot contribuir amb codi a Weavy, però us demanem que seguiu aquestes directrius per assegurar que les vostres contribucions puguin ser integrades sense problemes:

1. **Mantingueu les Pull Requests enfocades**

    - Limiteu les PR a una sola funcionalitat o correcció d'error
    - Dividiu els canvis més grans en PR més petites i relacionades
    - Dividiu els canvis en commits lògics que puguin ser revisats independentment

2. **Qualitat del codi**

    - Totes les PR han de passar les comprovacions de CI que inclouen tant anàlisi com formatació
    - Solucioneu qualsevol advertència o error d'ESLint abans d'enviar
    - Responeu a tots els comentaris d'Ellipsis, la nostra eina automatitzada de revisió de codi
    - Seguiu les millors pràctiques de TypeScript i mantingueu la seguretat de tipus

3. **Proves**

    - Afegiu proves per a noves funcionalitats
    - Executeu `npm test` per assegurar que totes les proves passin
    - Actualitzeu les proves existents si els vostres canvis les afecten
    - Incloeu tant proves unitàries com proves d'integració quan sigui apropiat

4. **Directrius de commits**

    - Escriviu missatges de commit clars i descriptius
    - Feu referència a incidències rellevants als commits utilitzant #número-incidència

5. **Abans d'enviar**

    - Rebaseu la vostra branca sobre l'última main
    - Assegureu-vos que la vostra branca es construeix amb èxit
    - Comproveu doblement que totes les proves passen
    - Reviseu els vostres canvis per qualsevol codi de depuració o registres de consola

6. **Descripció de la Pull Request**
    - Descriviu clarament què fan els vostres canvis
    - Incloeu passos per provar els canvis
    - Enumereu qualsevol canvi important
    - Afegiu captures de pantalla per a canvis d'interfície d'usuari

## Acord de contribució

En enviar una pull request, accepteu que les vostres contribucions estaran sota la mateixa llicència que el projecte ([Apache 2.0](../LICENSE)).
