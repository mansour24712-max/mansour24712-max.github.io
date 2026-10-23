# Setup docente — LAB01 — La mia identità tecnica su GitHub

Questo repository è un template riutilizzabile per un assignment individuale.
Non contiene riferimenti fissi a una classe, a studenti o a dati personali.

## Prima dell'uso: personalizzare i placeholder

Prima di pubblicare un assignment per una classe, sostituire in tutti i file i
tre placeholder seguenti:

| Placeholder | Esempio di valore |
| --- | --- |
| `{{CLASS_CODE}}` | `3BINF` |
| `{{CLASS_HUB_URL}}` | URL completo del Class Hub della classe |
| `{{TEACHER_GITHUB}}` | username GitHub del docente |

I placeholder compaiono in `README.md`, `STUDENT-GUIDE.md`,
`.github/ISSUE_TEMPLATE/lab01.yml` e nel materiale per il Class Hub. Dopo le
modifiche, controllare l'anteprima di ogni file Markdown e l'Issue Form.

## Configurazione del repository template

1. Creare nell'organizzazione `Torriani-AS2026` il repository
   `template-github-lab01-identita-tecnica`, con visibilità coerente con le
   politiche dell'istituto.
2. Caricare tutti i file di questo pacchetto nella radice del repository.
3. Aprire **Settings → General**.
4. Cercare la sezione **Template repository** e selezionare l'opzione per
   rendere il repository un template.
5. Aprire **Issues** e verificare che il modello
   **LAB01 — La mia identità tecnica su GitHub** sia selezionabile da **New issue**.
6. Se l'etichetta `lab01` non viene creata automaticamente, aprire
   **Issues → Labels → New label**, impostare nome `lab01` e salvare.

Non sono previste automazioni, valutazioni automatiche o altre configurazioni
aggiuntive per questo laboratorio.

## Creare il Class Hub di una classe

> Classroom50 non deve essere usato per creare il Class Hub: un assignment
> individuale genererebbe un repository distinto per ogni studente.

Per ogni classe, creare separatamente un repository condiviso, per esempio
`3BINF-github-hub` oppure `3DINF-github-hub`.

1. Nell'organizzazione, creare il repository del Class Hub con il nome della
   classe seguito da `-github-hub`.
2. Aggiungere un `README.md` copiando
   [`teacher/class-hub-starter/README.md`](teacher/class-hub-starter/README.md).
3. Sostituire `{{CLASS_CODE}}` e `{{TEACHER_GITHUB}}` nel README del Class Hub.
4. Aprire **Settings → General → Features** e abilitare **Discussions**.
5. Lasciare abilitate **Issues** se risultano utili alla classe.
6. Aprire **Discussions → New discussion** e creare:
   - `👋 Presentiamoci tecnicamente`;
   - `🆘 Aiuto LAB01`;
   - facoltativa: `💡 Idee e progetti che vorremmo realizzare`.
7. Copiare l'URL del Class Hub: sarà il valore di `{{CLASS_HUB_URL}}` per
   l'assignment di quella classe.

Verificare con un account studente che il Class Hub sia raggiungibile e che
possa leggere e rispondere alle Discussions secondo le impostazioni scelte.

# Configurazione Classroom50

Classroom50 usa un template repository come punto di partenza per i repository
degli studenti. Nel pannello di Classroom50, creare un nuovo assignment seguendo
la documentazione e l'interfaccia disponibili nell'istituto, con questa
configurazione concettuale:

| Campo | Valore |
| --- | --- |
| Organization | `Torriani-AS2026` |
| Classroom | una delle classi già configurate su Classroom50 |
| Assignment | `LAB01 - La mia identità tecnica su GitHub` |
| Type | individual |
| Template repository | `template-github-lab01-identita-tecnica` |

Non configurare autograding: non è un esercizio di programmazione.

## Procedura sicura quando i placeholder non sono sostituibili automaticamente

Non dare per scontato che Classroom50 sostituisca i placeholder nei file del
template. Se la sua interfaccia non offre una sostituzione documentata:

1. Dal template base selezionare **Use this template** e creare una variante
   temporanea per la classe, per esempio `template-github-lab01-3binf`.
2. Nel browser, sostituire i tre placeholder in tutti i file indicati nella
   sezione iniziale di questo documento.
3. Controllare l'anteprima Markdown e creare una Issue di prova per verificare
   che il form sia selezionabile e riporti l'URL corretto del Class Hub.
4. Selezionare la variante della classe come Template repository
   dell'assignment individuale in Classroom50.
5. Conservare invariato il template base, così da poter creare una nuova
   variante per un'altra classe o per un altro anno scolastico.

Se Classroom50 offre una procedura diversa documentata, applicare quella
procedura soltanto dopo aver verificato che il repository ricevuto da uno
studente contenga il corretto Class Hub della propria classe.

## Verifica prima della pubblicazione

- [ ] I tre placeholder sono stati sostituiti nella variante destinata alla classe.
- [ ] Il link del Class Hub apre il repository condiviso corretto.
- [ ] Discussions è abilitato nel Class Hub.
- [ ] Esistono le Discussions `👋 Presentiamoci tecnicamente` e `🆘 Aiuto LAB01`.
- [ ] L'Issue Form LAB01 è selezionabile da **Issues → New issue**.
- [ ] L'etichetta `lab01` esiste oppure la sua assenza è gestita consapevolmente.
- [ ] Il rendering Markdown è stato controllato nel browser.
- [ ] Nessun file contiene dati personali, credenziali, roster o riferimenti fissi a una classe.
- [ ] Il percorso è completabile nel browser senza installare software.
- [ ] Il testo non introduce concetti di versionamento non ancora trattati.

## Cosa osservare durante il laboratorio

Chiedere agli studenti di creare prima la propria Issue LAB01, poi di procedere
in ordine. La Issue è una scheda personale dell'attività, non un forum comune.
Le domande e le richieste di aiuto reali vanno nel Class Hub, nella Discussion
`🆘 Aiuto LAB01`. Gli studenti non devono chiudere autonomamente la Issue salvo
indicazione del docente.
