<script>
  import Header from "../components/Header.svelte";
</script>

<style type="text/scss">
	div {
		display: flex;
		text-align: center;
		justify-content: center;

		> div {
			color: var(--color-anthracite);
			padding: 1rem;
			margin: 0;
			border: 2px solid var(--color-light-grey);
			border-radius: 5px;
			box-shadow: 0 1px 6px -3px rgba(var(--color-light-grey), 0.2);
			display: flex;
			width: 324.656px;
			height: 244px;
			display: inline-flex;
			align-items: center;
			justify-content: center;

			&:first-of-type {
				margin-right: 2rem;
			}

			> a {
				text-decoration: none;
			}
		}
	}

	@media (max-width: 576px) {
        div {
			flex-direction: column;

			> div {
				&:first-of-type {
					margin-right: 0;
					margin-bottom: 2rem;
				}
			}
		}
    }
</style>

<svelte:head>
	<title>Integration</title>
</svelte:head>

<Header pageName={'Einbindung'} />
<h2>
	Machen Sie mit!
</h2>
<p>
	Auch Sie wollen Ihre Kundschaft und Nutzer*innen mit verifizierten Informationen über die aktuelle Covid19 Situation versorgen?
</p>
<p>
	Das freut uns!
</p>
<p>
	Unser Informations-Button ist ganz einfach auch auf Ihrer Internetseite einbindbar. Folgende Möglichkeiten können Sie hierzu nutzen:
</p>
<div>
	<div>
		<a href='https://github.com/coverified/webcomponent#simple-integration' rel="noopener" target="_blank">
			Unseren Code über JavaScript einbinden
		</a>
	</div>
	<div>
		<a href='https://github.com/coverified/plugin-wordpress' rel="noopener" target="_blank">
			Unseren Code bequem über unser Wordpress Plugin auf Ihrer Wordpresseite &ndash; oder Ihrem Blog einbinden.
		</a>
	</div>
</div>
<h2>
	So funktioniert der CoVerified Informations-Button auf Ihrer Website:
</h2>
<ul>
	<li>
		Unser CoVerified-Button erscheint immer unten rechts auf der Website und kann geöffnet werden.
	</li>
	<li>
		Mit einem Tipp oder Klick öffnet sich ein Fenster mit aktuellen Informationen zur Covid19-Krise.
	</li>
	<li>
		Wir zeigen die aktuellen Fallzahlen der John Hopkins University, so sind Sie immer informiert.
	</li>
	<li>
		Außerdem bereiten wir eine kleine Vorschau von Neuigkeiten auf, nur von staatlichen oder wissenschaftlich
		anerkannten Stellen.
	</li>
	<li>
		Die Vorschau der zugehörigen Artikel ist direkt auf die Quelle der Information verlinkt, damit Sie sich in
		Ruhe den ganzen Artikel durchlesen können.
	</li>
	<li>
		Barrierefreiheit: Unser Informations-Tool (auf Deutsch Werkzeug) nimmt die voreingestellte Schriftgröße des
		Browsers an, ist für Screenreading-Assistenten angepasst und soll auf lange Sicht auch mehrsprachig
		Informationen zur Verfügung stellen.
	</li>
</ul>
<h2>
	Unsere Datenbank
</h2>
<p>
	Unsere Datenbank wird gefüttert mit allen aktuellen Daten aus den RSS-Feeds offizieller Stellen. Diese Informationen
	werden gebündelt und als News-Vorschau in unserem Widget dargestellt. Klickt oder tippt der Nutzer auf ein solches
	Vorschau-Feld, wird er direkt zur aktuellen Meldung auf die Seite der jeweiligen Quelle weitergeleitet. <br/>
	Die Fallzahlen aktualisieren sich automatisch, durch eine Schnittstelle der John Hopkins University.
</p>
<h2>
	Helfen Sie mit!
</h2>
<p>
	Wir wollen zur besseren Information der Bevölkerung beitragen und proaktiv gegen die Verbreitung von Falschinformationen
	arbeiten. Wie wichtig stetige Information der Bevölkerung ist, sehen wir an vergangen Katastrophen oder jetzt im Zuge der
	Covid19-Krise auch vor allem am Beispiel von Südkorea.
</p>
<p>
	Bei technischen Fragen & Anregungen freuen wir uns über Ihren Kontakt.
	Melden Sie sich gerne via Mail, wir antworten so schnell wie möglich: info@coverified.info
</p>
