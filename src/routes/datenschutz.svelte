<script>
    import Header from '../components/Header.svelte';
    import Col from 'sveltestrap/src/Col.svelte';
    import Row from 'sveltestrap/src/Row.svelte';
</script>

<style type="text/scss">
    header {
        background-color: var(--color-primary);
        height: 14.6875rem;
        position: relative;
        justify-content: center;
        display: flex;
        margin-bottom: 3rem;

        &:before {
            content: "";
            position: absolute;
            background: var(--color-primary);
            display: block;
            width: 100vw;
            height: 100%;
            left: 50%;
            right: 0;
            bottom: 0;
            top: 0;
            transform: translateX(-50%);
        }
    }

    h1 {
        font-size: 2rem;
        position: absolute;
        color: var(--color-white);
        top: 8rem;
        left: 10rem;
    }

    .wirvsvirus__logo {
        position: absolute;
        width: 20rem;
        bottom: 37%;
        right: 1.125rem;
    }

    p {
        margin-bottom: 2.5rem;
    }

    @media (max-width: 768px) {
        header {
            flex-direction: column;
            align-items: center;
            justify-content: flex-start;

            > h1 {
                top: 3.5rem;
                left: unset;
            }

            > .wirvsvirus__logo {
                bottom: 1rem;
                right: auto;
                width: 15rem;
            }
        }
    }

    @media (max-width: 576px) {

    }
</style>

<svelte:head>
    <title>Impressum</title>
</svelte:head>
<header>
    <h1 class="sr-only">Impressum</h1>
    <h1>
        Datenschutzerklärung
    </h1>
    <img class="wirvsvirus__logo" src="wirvsvirus-weiss.svg" alt="Wir vs Virus Projekt">
</header>
<Row>
    <Col sm="auto" lg="12">
        <h2>Allgemeines</h2>
        <p>Die Einhaltung der Datenschutzgesetze ist f&uuml;r die&nbsp;Julia Diehl, Alessa Fetzer, Johannes Hiry, Steven
            Killian, Maximilian Mayer, Florian Schlittenbauer, Simon Schweikert, Christina Vollnhals, Paula Weise GbR
            nicht nur gesetzliche Pflicht, sondern auch ein wichtiger Vertrauensfaktor. Mit den nachfolgenden
            Datenschutzbestimmungen&nbsp;m&ouml;chten wir Sie deshalb transparent &uuml;ber Art, Umfang und Zweck der
            von Ihnen erhobenen und verarbeiteten personenbezogenen Daten innerhalb dieses Internetauftritts sowie Ihre
            Rechte informieren.&nbsp;</p>
        <h2>Verantwortlichkeit f&uuml;r die Datenverarbeitung</h2>
        <p>Die Julia Diehl, Alessa Fetzer, Johannes Hiry, Steven Killian, Maximilian Mayer, Florian Schlittenbauer,
            Simon Schweikert, Christina Vollnhals, Paula Weise GbR Ludwigstra&szlig;e 187 in 63067 Offenbach (Im
            Folgenden: &bdquo;Wir&ldquo;) ist als Betreiber der Webseite www.coverified.info, Verantwortlicher&nbsp;gem.&nbsp;Art.&nbsp;4&nbsp;Nr.&nbsp;7&nbsp;der
            EU-Datenschutz-Grundverordnung (DSGVO). Bei Fragen k&ouml;nnen Sie sich an&nbsp;
            <a href="mailto:info@coverified.info" title="E-Mail an info@coverified.info" target="_blank">info@coverified.info</a>
            wenden.</p>
        <h2>Datenschutzbeauftragter</h2>
        <p>Gem&auml;&szlig; Art.&nbsp;37 DSGVO i.V.m. &sect;&nbsp;38 BDSG sind wir nicht verpflichtet, einen
            Datenschutzbeauftragten zu bestellen. Bei Fragen zum Datenschutz und zur Geltendmachung Ihrer im folgenden
            genannten Rechte k&ouml;nnen Sie sich aber selbstverst&auml;ndlich jederzeit &uuml;ber die oben angegebenen
            Kontaktdaten an uns wenden.</p>
        <h2>Betroffenenrechte</h2>
        <h3>Ihre Rechte als betroffene Person</h3>
        <p>Als betroffene Person haben Sie uns gegen&uuml;ber folgende Rechte hinsichtlich Ihrer personenbezogenen
            Daten. Sie haben:</p>
        <ul>
            <li>Ein <strong>Recht auf&nbsp;Auskunft</strong>unter anderem &uuml;ber die Kategorien der verarbeiteten
                Daten, der Verarbeitungszwecke, die Speicherdauer sowie etwaige Empf&auml;nger, gem&auml;&szlig; Art.&nbsp;15
                DSGVO und &sect;&nbsp;34 BDSG.
            </li>
            <li>Ein <strong>Recht auf&nbsp;Berichtigung&nbsp;oder&nbsp;L&ouml;schung</strong>unrichtiger bzw. unvollst&auml;ndiger
                Daten, gem&auml;&szlig; Art.&nbsp;16 und 17 DSGVO und &sect;&nbsp;35 BDSG.
            </li>
            <li>Unter den Voraussetzungen des Art.&nbsp;18 DSGVO oder &sect;&nbsp;35 Abs.&nbsp;1 S.&nbsp;2 BDSG ein
                <strong>Recht auf&nbsp;Einschr&auml;nkung&nbsp;der Verarbeitung.</strong></li>
            <li>Ein <strong>Recht auf&nbsp;Widerspruch</strong>gegen die Verarbeitung gem&auml;&szlig; Art.&nbsp;21&nbsp;Abs.&nbsp;1
                DSGVO,&nbsp;soweit die Datenverarbeitung aufgrund eines berechtigten Interesses erfolgte.
            </li>
            <li>Ein <strong>Recht auf&nbsp;Widerruf</strong>einer abgegebenen Einwilligung mit Wirkung f&uuml;r die
                Zukunft gem&auml;&szlig; Art.&nbsp;7 Abs.&nbsp;3 DSGVO.
            </li>
            <li>Ein <strong>Recht auf&nbsp;Daten&uuml;bertragbarkeit</strong>in einem g&auml;ngigen Format gem&auml;&szlig;
                Art.&nbsp;20 DSGVO.
            </li>
            <li>Sie haben gem&auml;&szlig; Art.&nbsp;22 DSGVO ein <strong>Recht darauf, nicht einer ausschlie&szlig;lich
                auf einer automatisierten Verarbeitung beruhenden Entscheidung unterworfen zu werden</strong>, die Ihnen
                gegen&uuml;ber rechtliche Wirkung entfaltet oder Sie in &auml;hnlicher Weise erheblich beeintr&auml;chtigt.
                Dies umfasst auch Profiling im Sinne des Art.&nbsp;4 Nr.&nbsp;4 DSGVO.
            </li>
            <li>Sie haben zudem das Recht, sich gem&auml;&szlig; Art.&nbsp;77 DSGVO bei einer <strong>Datenschutz-Aufsichtsbeh&ouml;rde</strong>
                &uuml;ber die Verarbeitung Ihrer personenbezogenen Daten durch uns zu beschweren, insbesondere in dem
                Mitgliedstaat Ihres gew&ouml;hnlichen Aufenthaltsorts, Ihres Arbeitsplatzes oder des Orts des mutma&szlig;lichen
                Versto&szlig;es.
            </li>
        </ul>
        <h3>Verfahren</h3>
        <p>Wenn Sie Ihre Rechte nach der DSGVO und dem BDSG uns gegen&uuml;ber geltend machen, werden wir die von Ihnen
            dabei an uns &uuml;bermittelten Daten verarbeiten, um Ihren Anspruch zu erf&uuml;llen.</p>
        <p>Im Anschluss speichern wir die von Ihnen an uns &uuml;bermittelten Daten und die von uns an Sie im Gegenzug
            &uuml;bermittelten Daten zum Zwecke der Dokumentation bis zum Ablauf der ordnungswidrigkeitenrechtlichen
            Verj&auml;hrungsfrist (3 Jahre).</p>
        <p>Die Rechtsgrundlage f&uuml;r die Verarbeitung und Speicherung der Daten ist Art.&nbsp;6 Abs.&nbsp;1 S.&nbsp;1
            Buchstabe&nbsp;f) DSGVO (Berechtigtes Interesse an der Datenverarbeitung). Das berechtigte Interesse ergibt
            sich aus unserer Verpflichtung Ihrem Anliegen nachzukommen und dem Bedarf, uns in einem m&ouml;glichen Bu&szlig;geldverfahren
            entlasten zu k&ouml;nnen, indem wir nachweisen, dass wir Ihrem Anliegen ordnungsgem&auml;&szlig;
            nachgekommen sind.</p>
        <p>Der Verarbeitung Ihrer Daten auf Grundlage unseres berechtigten Interesses k&ouml;nnen Sie jederzeit unter
            den Voraussetzungen des Art.&nbsp;21 DSGVO widersprechen. Nutzen Sie hierf&uuml;r bitte die im Impressum
            genannten Kontaktdaten. Wir weisen aber darauf hin, dass die Verarbeitung Ihrer Daten zum Nachweis der
            Einhaltung der Betroffenenrechte zwingend im Sinne des Art.&nbsp;21 Abs.&nbsp;1 DSGVO ist, da andere
            Nachweism&ouml;glichkeiten nicht bestehen bzw. nicht gleicherma&szlig;en geeignet sind.</p>
        <h2>Datenschutzma&szlig;nahmen</h2>
        <p>Wir sichern unsere Webseite und sonstigen Systeme &ndash; und damit auch Ihre Daten &ndash; durch technische
            und organisatorische Ma&szlig;nahmen gegen Verlust, Zerst&ouml;rung, Zugriff, Ver&auml;nderung oder
            Verbreitung durch unbefugte Personen ab. Insbesondere werden Ihre pers&ouml;nlichen Daten verschl&uuml;sselt
            durch das Internet &uuml;bertragen. Wir bedienen uns dabei des Codierungssystems&nbsp;TLS (Transport Layer
            Security).</p>
        <p>Jedoch ist die &Uuml;bertragung von Informationen &uuml;ber das Internet nie vollst&auml;ndig sicher, weshalb
            wir die Sicherheit der von unserer Webseite &uuml;bermittelten Daten nicht zu 100% garantieren
            k&ouml;nnen.</p>
        <h2>Modalit&auml;ten der Datenverarbeitung</h2>
        <h3>Quellen und Kategorien von personenbezogenen Daten</h3>
        <p>Wir verarbeiten Ihre personenbezogenen Daten, soweit sie f&uuml;r die Begr&uuml;ndung, inhaltliche
            Ausgestaltung oder &Auml;nderung eines Vertragsverh&auml;ltnisses zwischen uns und Ihnen erforderlich sind
            (Bestandsdaten). Bestandsdaten k&ouml;nnen insbesondere sein: Name, Anrede, Kontaktdaten (Postadresse,
            Telefon, E-Mail-Adresse), Geburtsdatum usw.</p>
        <p>Ferner verarbeiten wir Ihre Nutzungsdaten. Nutzungsdaten sind Daten, die durch Ihr Verhalten bei der Nutzung
            unseres Webangebots und unserer Dienste anfallen, insbesondere Ihre IP-Adresse, Beginn und Ende Ihres
            Besuchs auf unserer Webseite und Informationen dar&uuml;ber, welche Inhalte Sie auf unserer Webseite
            abgerufen haben.</p>
        <p>Die genannten Daten erheben wir entweder direkt bei Ihnen (z.B. durch den Besuch der Webseite) oder, soweit
            dies nach den Datenschutzgesetzen zul&auml;ssig ist, bei Dritten bzw. aus &ouml;ffentlich zug&auml;nglichen
            Quellen (z.B. Handels- und Vereinsregister, Presse, Medien, Internet).</p>
        <h3>Daten&uuml;bermittlung an Drittstaaten au&szlig;erhalb der EU</h3>
        <p>Alle Informationen, die wir von Ihnen oder &uuml;ber Sie erhalten, werden grunds&auml;tzlich auf Servern
            innerhalb der Europ&auml;ischen Union verarbeitet. Eine &Uuml;bermittlung Ihrer Daten an oder eine
            Verarbeitung Ihrer Daten in Drittstaaten erfolgt ohne Ihre ausdr&uuml;ckliche Einwilligung lediglich, sofern
            dies gesetzlich vorgesehen oder gestattet ist und in dem Drittstaat ein hierf&uuml;r angemessenes
            Datenschutzniveau sichergestellt ist.&nbsp;</p>
        <h3>Weitergabe von Daten, Auftragsverarbeitung</h3>
        <p>Wir geben Ihre personenbezogenen Daten niemals unberechtigt an Dritte weiter. Wir k&ouml;nnen Ihre Daten aber
            insbesondere an Dritte weitergeben, wenn Sie in die Datenweitergabe eingewilligt haben, wenn die Weitergabe
            zur Erf&uuml;llung unserer rechtlichen Verpflichtungen notwendig ist oder wenn wir aufgrund gesetzlicher
            Bestimmungen oder beh&ouml;rdlicher oder gerichtlicher Anordnungen zu einer Datenweitergabe berechtigt oder
            verpflichtet sind. Dabei kann es sich insbesondere um die Auskunftserteilung f&uuml;r Zwecke der
            Strafverfolgung, zur Gefahrenabwehr oder zur Durchsetzung geistiger Eigentumsrechte handeln.</p>
        <p>Unter Umst&auml;nden &uuml;bermitteln wir Ihre Daten au&szlig;erdem an externe Dienstleister, die Daten in
            unserem Auftrag und nach unserer Weisung verarbeiten (Auftragsverarbeiter), um unsere eigene
            Datenverarbeitung zu vereinfachen oder zu entlasten. Jeder Auftragsverarbeiter wird durch einen Vertrag nach
            Ma&szlig;gabe des Art.&nbsp;28 DSGVO verpflichtet. Das hei&szlig;t insbesondere, dass der
            Auftragsverarbeiter hinreichend Garantien daf&uuml;r zu bieten hat, dass durch ihn geeignete technische und
            organisatorische Ma&szlig;nahmen so durchgef&uuml;hrt werden, dass die Verarbeitung im Einklang mit den
            Anforderungen der DSGVO erfolgt und der Schutz Ihrer Rechte als betroffene Person gew&auml;hrleistet ist.
            Trotz Beauftragung von Auftragsverarbeitern bleiben wir f&uuml;r die Verarbeitung Ihrer personenbezogenen
            Daten die verantwortliche Stelle im Sinne der Datenschutzgesetze.</p>
        <h3>Zweck der Datenverarbeitung</h3>
        <p>Wir nutzen die Daten grunds&auml;tzlich nur zu dem Zweck, zu dem die Daten von Ihnen erhoben wurden. Wir k&ouml;nnen
            die Daten zu einem anderen Zweck weiterverarbeiten, wenn nicht dieser andere Zweck mit dem urspr&uuml;nglichen
            Zweck unvereinbar ist (Art.&nbsp;5 Abs.&nbsp;1 Lit. c) DSGVO).</p>
        <h3>Speicherdauer</h3>
        <p>Soweit im Einzelnen nichts anderes angegeben ist, speichern wir von Ihnen erhobene Daten nur so lange, wie es
            f&uuml;r den jeweiligen Zweck erforderlich ist, es sei denn es stehen gesetzliche Aufbewahrungspflichten der
            L&ouml;schung entgegen, z.B. aus dem Handelsrecht oder dem Steuerrecht.</p>
        <h2>Einzelne Verarbeitungst&auml;tigkeiten</h2>
        <p>Wir m&ouml;chten Ihnen im Folgenden so transparent wie m&ouml;glich darstellen, welche Daten wir von Ihnen zu
            welcher Gelegenheit, auf welcher Grundlage und zu welchem Zweck verarbeiten.</p>
        <h3>Server-Log-Dateien</h3>
        <p>Bei jedem&nbsp;Aufruf einer Webseite und bei jedem Abruf von Daten von einem Server&nbsp;werden allgemeine
            Informationen automatisch an den bereitstellenden Server &uuml;bermittelt. Diese Daten&uuml;bermittlung
            erfolgt automatisch und ist ein grundlegender Bestandteil der Kommunikation zwischen Ger&auml;ten im
            Internet.</p>
        <p>Die standardm&auml;&szlig;ig &uuml;bertragenen Daten umfassen unter anderem folgende Informationen: Ihre
            IP-Adresse,&nbsp;Produkt- und Versionsinformationen &uuml;ber den verwendeten Browser und das Betriebssystem
            (sog. user agent), die&nbsp;Internetseite von welcher Ihr&nbsp;Zugriff&nbsp;stattfand (sog. referer), Datum
            und Uhrzeit der Anfrage (sog. timestamp). Au&szlig;erdem werden der http-Status und die &uuml;bertragene
            Datenmenge im Rahmen dieser Anfrage erfasst.</p>
        <p>Diese Informationen werden vom Server protokolliert, in einer Tabelle abgelegt und dort kurzfristig
            gespeichert (sog. Server-Log-Dateien). Durch die Analyse dieser Log-Dateien k&ouml;nnen wir Fehler der
            Webseite feststellen und anschlie&szlig;end beseitigen, die Auslastung der Webseite zu bestimmten Zeiten
            feststellen und darauf aufbauend Anpassungen oder Verbesserungen vornehmen sowie die Sicherheit des Servers
            gew&auml;hrleisten, indem wir nachvollziehen k&ouml;nnen, von welcher IP-Adresse Angriffe auf unseren Server
            ausgef&uuml;hrt wurden.</p>
        <p>Ihre IP-Adresse wird nur f&uuml;r die Zeit Ihrer Nutzung der Webseite gespeichert&nbsp;und im Anschluss daran
            unverz&uuml;glich gel&ouml;scht oder durch K&uuml;rzung teilweise unkenntlich gemacht. Die &uuml;brigen
            Daten werden f&uuml;r eine begrenzte Zeitdauer (meist 7 Tage) gespeichert.</p>
        <p>Die Rechtsgrundlage f&uuml;r die Nutzung der Server-Log-Dateien ist Art.&nbsp;6 Abs.&nbsp;1 S.&nbsp;1
            Buchstabe&nbsp;f) DSGVO (Berechtigtes Interesse an der Datenverarbeitung). Das berechtigte Interesse ergibt
            sich aus der Notwendigkeit f&uuml;r den Betrieb und die Wartung unserer Webseite, wie wir vorstehend erl&auml;utert
            haben. Der Verarbeitung Ihrer Daten auf Grundlage unseres berechtigten Interesses k&ouml;nnen Sie jederzeit
            unter den Voraussetzungen des Art.&nbsp;21 DSGVO widersprechen. Nutzen Sie hierf&uuml;r bitte die im
            Impressum genannten Kontaktdaten. Wir weisen aber bereits im Vorfeld darauf hin, dass die Verarbeitung Ihrer
            Daten in Server-Log-Dateien zwingend im Sinne des Art.&nbsp;21 Abs.&nbsp;1 DSGVO ist, da die Webseite
            ansonsten &uuml;berhaupt nicht betrieben werden kann.</p>
        <h3>Cookies und Web Storage</h3>
        <p>Unsere Webseite nutzt keine Cookies und greift nicht auf den Web Storage Ihres Browsers zu.</p>
        <h2>Dienste Dritter</h2>
        <p>Wir nutzen, zur Vereinfachung unserer Datenverarbeitung und um den Funktionsumfang unserer Webseite zu
            erweitern, Dienstleistungen/Ressourcen von Dritten, beispielsweise Plugins, externe Inhalte, Software oder
            sonstige externe Dienstleister (Dienste). Dabei werden m&ouml;glicherweise auch personenbezogene Daten an
            den Diensteanbieter &uuml;bermittelt. Um Ihre Daten zu sch&uuml;tzen, haben wir die Diensteanbieter
            erforderlichenfalls gem. Art.&nbsp;28 DSGVO vertraglich verpflichtet, Ihre Daten nur nach unserer Anweisung
            zu verarbeiten.</p>
        <p>Wir weisen ausdr&uuml;cklich darauf hin, dass wir regelm&auml;&szlig;ig nur f&uuml;r die Datenerhebung und
            &Uuml;bermittlung durch den Dienst verantwortlich im Sinne der DSGVO sind, nicht aber f&uuml;r eine
            eventuell sp&auml;ter erfolgende Verarbeitung durch den jeweiligen Diensteanbieter.</p>
        <p>Im Einzelnen nutzen wir folgende Dienste:</p>
        <h3>Content Delivery Networks</h3>
        <p>Unsere Webseite bedient sich sogenannter Content Delivery Networks (CDN). Ein CDN ist ein Netzwerk aus
            leistungsf&auml;higen Servern, die Inhalte an verschiedenen Orten auf der ganzen Welt zwischenspeichern.
            Dabei hat ein CDN im Wesentlichen zwei Aufgaben: zum einen soll es Inhalte in k&uuml;rzester Zeit
            bereitstellen und zum anderen den Web-Host entlasten, indem der Datenverkehr verteilt wird.</p>
        <p>CDNs &uuml;bermitteln zwei Arten von Inhalten: Statische und dynamische Inhalte. Statische Inhalte erhalten
            alle Webseitenbesucher in gleicher Form, wie zum Beispiel Videoinhalte von Streaming-Diensten oder
            Code-Frameworks (z.B. Javascript, jQuery). Dynamische Inhalte werden zun&auml;chst an den Nutzer angepasst
            und erst im Moment der Anfrage erstellt. Dazu z&auml;hlen Inhalte, die &uuml;ber Web-Anwendungen, E-Mail
            oder Online-Shops erfolgen und personalisiert sind. Um letzteres nutzen zu k&ouml;nnen, m&uuml;ssen erst
            Informationen &uuml;ber den Webseitenbesucher an das CDN &uuml;bermittelt werden. Hierbei k&ouml;nnen auch
            pers&ouml;nliche Daten von Ihnen &uuml;bermittelt werden.</p>
        <p>Bei jedem&nbsp;Aufruf der Anwendung&nbsp;werden allgemeine Informationen von Ihrem Browser automatisch an den
            Server &uuml;bermittelt (sog. Server-Log-Dateien). N&auml;here Informationen hierzu siehe oben unter &bdquo;Server-Log-Dateien&ldquo;.</p>
        <p>Die Rechtsgrundlage f&uuml;r die Nutzung von CDNs und die &Uuml;bermittlung Ihrer Daten an diese ist Art.&nbsp;6
            Abs.&nbsp;1 S.&nbsp;1 Buchstabe&nbsp;f) DSGVO (Berechtigtes Interesse an der Datenverarbeitung), soweit bei
            dem jeweiligen Dienst nichts anderes angegeben ist. Das berechtigte Interesse ergibt sich aus unserem Bedarf
            an einer technisch einwandfreien und schnellen Darstellung unserer Webseite und der Entlastung unserer
            IT-Infrastruktur. Der Verarbeitung Ihrer Daten auf Grundlage unseres berechtigten Interesses k&ouml;nnen Sie
            jederzeit unter den Voraussetzungen des Art.&nbsp;21 DSGVO widersprechen. Nutzen Sie hierf&uuml;r bitte die
            im Impressum genannten Kontaktdaten.</p>
        <p>Wir verwenden:</p>
        <h4>Amazon Web Services &ndash; Cloudfront</h4>
        <p>Wir nutzen den CDN-Dienst &bdquo;Cloudfront&ldquo; von Amazon Web Services. Die Firma Amazon Web Services
            EMEA SARL (&bdquo;AWS EU&ldquo;), 38 Avenue John F. Kennedy, L-1855 Luxemburg, ist die Verantwortliche f&uuml;r
            personenbezogene Daten, die &uuml;ber die Angebote von &bdquo;Amazon Web Services&ldquo; erhoben und
            verarbeitet werden. AWS EU ist die autorisierte Vertreterin der Amazon Web Services Inc. (&bdquo;AWS US&ldquo;),
            410 Terry Avenue North, Seattle WA 98109, United States.</p>
        <p>Durch die Nutzung der Dienste werden Daten an AWS EU und unter Umst&auml;nden von AWS EU an AWS US &uuml;bermittelt.
            Der Amazon-Konzern kann die &uuml;bermittelten Daten verarbeiten, um anonymisierte Nutzerprofile f&uuml;r
            statistische Zwecke zu erstellen. Auf diese Datenverarbeitung haben wir grunds&auml;tzlich keinen Einfluss.
            Verantwortlich f&uuml;r diese Datenverarbeitung ist daher AWS EU.</p>
        <p>Mehr Informationen zum Umgang mit Nutzerdaten finden Sie in der Datenschutzerkl&auml;rung von AWS EU unter
            <a href="https://aws.amazon.com/de/privacy/?nc1=f_pr"
               title="https://aws.amazon.com/de/privacy/?nc1=f_pr"
               rel="noopener"
               target="_blank"
            >https://aws.amazon.com/de/privacy/?nc1=f_pr</a>.
        </p>
        <h4>Bootstrap</h4>
        <p>Wir nutzen den CDN-Dienst &bdquo;BootstrapCDN&ldquo; (auch &bdquo;MaxCDN&ldquo; genannt) der Firma StackPath
            LLC (&bdquo;StackPath&ldquo;), 2021 McKinney Ave., Suite 1100, Dallas, TX 75201, USA.</p>
        <p>Mehr Informationen zum Umgang mit Nutzerdaten finden Sie in der Datenschutzerkl&auml;rung von StackPath:
            <a href="https://www.stackpath.com/privacy-statement/"
               title="https://www.stackpath.com/privacy-statement/"
               rel="noopener"
               target="_blank"
            >https://www.stackpath.com/privacy-statement/</a>
            oder in der Datenschutzerkl&auml;rung von BootstrapCDN:
            <a href="https://www.bootstrapcdn.com/privacy-policy/"
               title="https://www.bootstrapcdn.com/privacy-policy/"
               rel="noopener"
               target="_blank"
            >https://www.bootstrapcdn.com/privacy-policy/</a>.
        </p>
        <h2>Social-Media-Fanseiten</h2>
        <p>Zus&auml;tzlich zu unserer Webseite unterhalten wir Onlinepr&auml;senzen auf sozialen Plattformen, um mit den
            dort aktiven Kunden, Interessenten und Nutzern kommunizieren und sie dort &uuml;ber unsere Leistungen
            informieren zu k&ouml;nnen.</p>
        <p>Wenn Sie unsere Pr&auml;senz auf einer sozialen Plattform besuchen, werden Ihre Daten im Regelfall f&uuml;r
            unsere Marktforschungs- und Werbezwecke von dem jeweiligen Anbieter der Plattform verarbeitet. Der Anbieter
            kann die Daten auch f&uuml;r eigene Zwecke verarbeiten. Aus Ihrem Nutzungsverhalten und Ihrer sich daraus
            ergebenden Interessen k&ouml;nnen Nutzungsprofile erstellt werden. Diese Nutzungsprofile k&ouml;nnen
            wiederum verwendet werden, um z.B. Werbeanzeigen innerhalb und au&szlig;erhalb der Plattformen zu schalten,
            die mutma&szlig;lich Ihren Interessen entsprechen. Zu diesen Zwecken werden im Regelfall Cookies (siehe
            oben) auf Ihrem Endger&auml;t gespeichert, in denen Ihr Nutzungsverhalten und Ihre Interessen gespeichert
            werden. Insbesondere wenn Sie Mitglied der jeweiligen Plattformen sind und bei diesen eingeloggt sind, k&ouml;nnen
            in den Nutzungsprofilen noch zus&auml;tzliche Daten unabh&auml;ngig gespeichert werden. F&uuml;r eine
            detaillierte Darstellung der jeweiligen Datenverarbeitung und der Widerspruchsm&ouml;glichkeiten, verweisen
            wir auf die nachfolgend verlinkten Angaben der Anbieter, da nur diese die genauen Abl&auml;ufe ihrer
            Datenverarbeitung kennen.</p>
        <p>Wir weisen darauf hin, dass Ihre Daten auch au&szlig;erhalb der Europ&auml;ischen Union verarbeitet werden k&ouml;nnen.
            Hierdurch k&ouml;nnen Risiken ergeben, weil so z.B. die Durchsetzung Ihrer Rechte erschwert werden k&ouml;nnte.</p>
        <p>Die Rechtsgrundlage f&uuml;r die Nutzung der Onlinepr&auml;senzen und der damit verbundenen Datenverarbeitung
            ist im Allgemeinen Art.&nbsp;6 Abs.&nbsp;1 S.&nbsp;1 Buchstabe&nbsp;f) DSGVO (Berechtigtes Interesse an der
            Datenverarbeitung). Das berechtigte Interesse ergibt sich aus unserem Bedarf uns den Besuchern und Nutzern
            der sozialen Netzwerke zu pr&auml;sentieren und &Auml;u&szlig;erungen aller Art in den Medien- und
            Meinungsmarkt einzubringen. Der Verarbeitung Ihrer Daten auf Grundlage unseres berechtigten Interesses k&ouml;nnen
            Sie jederzeit unter den Voraussetzungen des Art.&nbsp;21 DSGVO widersprechen. Nutzen Sie hierf&uuml;r bitte
            die im Impressum genannten Kontaktdaten.</p>
        <p>Die Nutzung von statistischen Daten aller Besucher unserer Social-Media-Webpr&auml;senzen, die f&uuml;r uns
            von den jeweiligen Seitenbetreibern erhoben, aufbereitet und zur Verf&uuml;gung gestellt werden beruht auf
            Art.&nbsp;6 Abs.&nbsp;1 S.&nbsp;1 Buchstabe&nbsp;f) DSGVO (Berechtigtes Interesse an der Datenverarbeitung).
            Das berechtigte Interesse ergibt sich aus unserem Bedarf an einer anonymen Auswertung des Besuchs- und
            Nutzungsverhaltens auf unseren Webpr&auml;senzen zur nutzungsorientierten Verbesserung der Gestaltung
            unseres Online-Angebots und der Optimierung unserer Kommunikation mit Interessenten. Der Verarbeitung Ihrer
            Daten auf Grundlage unseres berechtigten Interesses k&ouml;nnen Sie jederzeit unter den Voraussetzungen des
            Art.&nbsp;21 DSGVO widersprechen. Nutzen Sie hierf&uuml;r bitte die im Impressum genannten Kontaktdaten.</p>
        <p>Falls Sie von den jeweiligen Anbietern um eine Einwilligung in die Datenverarbeitung gebeten werden, ist die
            Rechtsgrundlage f&uuml;r die Verarbeitung Art.&nbsp;6 Abs.&nbsp;1 S.&nbsp;1 Buchstabe&nbsp;a) DSGVO
            (Einwilligung der betroffenen Person). Diese Einwilligung k&ouml;nnen Sie jederzeit mit Wirkung f&uuml;r die
            Zukunft widerrufen. Kontaktieren Sie hierf&uuml;r bitte den Anbieter, der Sie um Ihre Einwilligung gebeten
            hat.</p>
        <p>F&uuml;r den Fall, dass Sie Ihre oben genannten Rechte geltend machen wollen, weisen wir darauf hin, dass
            diese, trotz eventueller gemeinsamer Verantwortlichkeit, am effektivsten bei den Anbietern geltend gemacht
            werden k&ouml;nnen. In der Regel haben nur die Anbieter unmittelbaren Zugriff auf Ihre Daten und k&ouml;nnen
            direkt entsprechende Ma&szlig;nahmen ergreifen und Ausk&uuml;nfte geben. Sollten Sie dennoch Hilfe ben&ouml;tigen,
            dann k&ouml;nnen Sie sich an uns wenden und wir werden Sie jederzeit im Rahmen unserer M&ouml;glichkeiten
            unterst&uuml;tzen.</p>
        <p>Wir sind vertreten auf:</p>
        <h3><em>Twitter</em></h3>
        <p>Twitter ist ein soziales Netzwerk der Twitter International Company, One Cumberland Place, Fenian Street,
            Dublin 2, D02 AX07, Ireland. Die Firma Twitter International Company ist die europ&auml;ische Tochter der
            Firma Twitter Inc.,1355 Market Street, Suite 900, San Francisco, CA 94103, USA.</p>
        <p>Weitere Informationen zum Datenschutz bei Twitter finden Sie unter:&nbsp;
            <a href="https://twitter.com/de/privacy"
               title="https://twitter.com/de/privacy"
               rel="noopener"
               target="_blank"
            >https://twitter.com/de/privacy</a>.
        </p>
        <p>Die Datenerhebung von Twitter k&ouml;nnen Sie auf der folgenden Seite konfigurieren:
            <a href="https://twitter.com/personalization"
               title="https://twitter.com/personalization"
               rel="noopener"
               target="_blank"
            >https://twitter.com/personalization</a>
        </p>
        <p>&nbsp;</p>
        <p>Stand der Datenschutzerkl&auml;rung: 15.10.2020</p>
        <p>Quelle:&nbsp;
            <a href="http://www.sddsg.de/"
               title="http://www.sddsg.de/"
               rel="noopener"
               target="_blank"
            >S&uuml;ddeutsche Datenschutzgesellschaft mbH</a>
        </p>
    </Col>
</Row>
