<html lang="cs">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FitFactory – Privacy Policy / Zásady ochrany osobních údajů</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg: #FAFAF9;
            --surface: #FFFFFF;
            --text: #1C1917;
            --text-secondary: #57534E;
            --accent: #EA580C;
            --accent-light: #FFF7ED;
            --border: #E7E5E4;
            --radius: 12px;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            font-family: 'DM Sans', -apple-system, BlinkMacSystemFont, sans-serif;
            background: var(--bg);
            color: var(--text);
            line-height: 1.7;
            font-size: 16px;
        }

        .container {
            max-width: 720px;
            margin: 0 auto;
            padding: 40px 24px 80px;
        }

        /* Header */
        .header {
            text-align: center;
            margin-bottom: 48px;
            padding-bottom: 32px;
            border-bottom: 1px solid var(--border);
        }

        .logo {
            font-size: 28px;
            font-weight: 700;
            color: var(--accent);
            letter-spacing: -0.5px;
            margin-bottom: 8px;
        }

        .header h1 {
            font-size: 22px;
            font-weight: 600;
            color: var(--text);
            margin-bottom: 12px;
        }

        .lang-switch {
            display: inline-flex;
            background: var(--surface);
            border: 1px solid var(--border);
            border-radius: 8px;
            overflow: hidden;
            margin-top: 8px;
        }

        .lang-btn {
            padding: 8px 20px;
            border: none;
            background: transparent;
            font-family: inherit;
            font-size: 14px;
            font-weight: 500;
            color: var(--text-secondary);
            cursor: pointer;
            transition: all 0.2s;
        }

        .lang-btn.active {
            background: var(--accent);
            color: white;
        }

        .lang-btn:hover:not(.active) {
            background: var(--accent-light);
            color: var(--accent);
        }

        /* Content */
        .effective-date {
            font-size: 14px;
            color: var(--text-secondary);
            margin-bottom: 32px;
        }

        section {
            margin-bottom: 32px;
        }

        h2 {
            font-size: 18px;
            font-weight: 600;
            color: var(--text);
            margin-bottom: 12px;
            padding-top: 8px;
        }

        p {
            margin-bottom: 12px;
            color: var(--text-secondary);
        }

        .data-table {
            width: 100%;
            border-collapse: collapse;
            margin: 16px 0;
            background: var(--surface);
            border-radius: var(--radius);
            overflow: hidden;
            border: 1px solid var(--border);
        }

        .data-table th {
            background: var(--accent-light);
            color: var(--accent);
            font-weight: 600;
            font-size: 13px;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            padding: 12px 16px;
            text-align: left;
        }

        .data-table td {
            padding: 12px 16px;
            border-top: 1px solid var(--border);
            color: var(--text-secondary);
            font-size: 14px;
        }

        .data-table tr:hover td {
            background: var(--accent-light);
        }

        .highlight-box {
            background: var(--accent-light);
            border-left: 3px solid var(--accent);
            padding: 16px 20px;
            border-radius: 0 var(--radius) var(--radius) 0;
            margin: 16px 0;
        }

        .highlight-box p {
            color: var(--text);
            margin: 0;
        }

        .contact-box {
            background: var(--surface);
            border: 1px solid var(--border);
            border-radius: var(--radius);
            padding: 24px;
            text-align: center;
            margin-top: 40px;
        }

        .contact-box a {
            color: var(--accent);
            font-weight: 600;
            text-decoration: none;
        }

        .contact-box a:hover {
            text-decoration: underline;
        }

        .footer {
            text-align: center;
            margin-top: 48px;
            padding-top: 24px;
            border-top: 1px solid var(--border);
            font-size: 13px;
            color: var(--text-secondary);
        }

        .content-section { display: none; }
        .content-section.active { display: block; }

        @media (max-width: 480px) {
            .container { padding: 24px 16px 60px; }
            .logo { font-size: 24px; }
            .header h1 { font-size: 18px; }
            .data-table { font-size: 13px; }
            .data-table th, .data-table td { padding: 10px 12px; }
        }
    </style>
</head>
<body>

<div class="container">
    <div class="header">
        <div class="logo">FitFactory</div>
        <h1 id="page-title">Zásady ochrany osobních údajů</h1>
        <div class="lang-switch">
            <button class="lang-btn active" onclick="switchLang('cs')" id="btn-cs">Česky</button>
            <button class="lang-btn" onclick="switchLang('en')" id="btn-en">English</button>
        </div>
    </div>

    <!-- CZECH VERSION -->
    <div class="content-section active" id="content-cs">
        <p class="effective-date">Platné od: 1. března 2026</p>

        <section>
            <h2>1. Úvod</h2>
            <p>FitFactory („aplikace") je mobilní aplikace pro sledování silových tréninků. Vaše soukromí je pro nás důležité. Tyto zásady popisují, jaké údaje sbíráme, jak je používáme a jak je chráníme.</p>
        </section>

        <section>
            <h2>2. Jaké údaje sbíráme</h2>

            <table class="data-table">
                <thead>
                    <tr>
                        <th>Typ údaje</th>
                        <th>Účel</th>
                        <th>Uložení</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Email a heslo</td>
                        <td>Registrace a přihlášení</td>
                        <td>Firebase Authentication (Google Cloud)</td>
                    </tr>
                    <tr>
                        <td>Zobrazované jméno</td>
                        <td>Identifikace v aplikaci</td>
                        <td>Firebase Firestore</td>
                    </tr>
                    <tr>
                        <td>Přezdívka</td>
                        <td>Vyhledávání uživatelů</td>
                        <td>Firebase Firestore</td>
                    </tr>
                    <tr>
                        <td>Profilová fotka</td>
                        <td>Volitelná personalizace</td>
                        <td>Firebase Storage</td>
                    </tr>
                    <tr>
                        <td>Tréninková data</td>
                        <td>Sledování pokroku</td>
                        <td>Lokálně v zařízení</td>
                    </tr>
                    <tr>
                        <td>Osobní maxima</td>
                        <td>Výpočet tréninkových vah</td>
                        <td>Lokálně v zařízení</td>
                    </tr>
                </tbody>
            </table>

            <div class="highlight-box">
                <p><strong>Důležité:</strong> Vaše tréninková data (tréninky, série, váhy, osobní maxima) jsou uložena výhradně lokálně ve vašem zařízení. Na naše servery se neodesílají, pokud sami nevyužijete funkci sdílení s trenérem.</p>
            </div>
        </section>

        <section>
            <h2>3. Jak údaje používáme</h2>
            <p>Vaše údaje používáme výhradně pro:</p>
            <p>• Autentizaci a správu vašeho účtu</p>
            <p>• Komunikaci mezi trenérem a klientem (pokud tuto funkci využíváte)</p>
            <p>• Sdílení tréninků a notifikace v rámci trenér-klient systému</p>
            <p>• Zlepšování aplikace na základě anonymní agregované statistiky</p>
        </section>

        <section>
            <h2>4. Sdílení údajů s třetími stranami</h2>
            <p>Vaše osobní údaje <strong>neprodáváme ani nesdílíme</strong> s třetími stranami za účelem reklamy nebo marketingu.</p>
            <p>Údaje sdílíme pouze v těchto případech:</p>
            <p>• <strong>Firebase / Google Cloud</strong> – pro provoz autentizace a cloudových služeb (v souladu s podmínkami Google Cloud)</p>
            <p>• <strong>Trenér-klient</strong> – vaše tréninková data se sdílejí s trenérem pouze na základě vašeho výslovného souhlasu (přijetí žádosti o připojení)</p>
        </section>

        <section>
            <h2>5. Zabezpečení</h2>
            <p>Veškerá komunikace mezi aplikací a servery je šifrována (HTTPS/TLS). Firebase Authentication zajišťuje bezpečné ukládání přihlašovacích údajů. Přístup k datům v cloudové databázi je řízen bezpečnostními pravidly Firebase.</p>
        </section>

        <section>
            <h2>6. Vaše práva</h2>
            <p>Máte právo:</p>
            <p>• <strong>Přistupovat</strong> ke svým údajům uloženým v aplikaci</p>
            <p>• <strong>Opravit</strong> své osobní údaje v nastavení profilu</p>
            <p>• <strong>Smazat</strong> svůj účet a veškerá asociovaná cloudová data</p>
            <p>• <strong>Exportovat</strong> svá tréninková data (funkce backup)</p>
            <p>Lokální tréninková data se smažou odinstalací aplikace.</p>
        </section>

        <section>
            <h2>7. Děti</h2>
            <p>Aplikace FitFactory není určena pro děti mladší 16 let. Vědomě nesbíráme údaje od osob mladších 16 let.</p>
        </section>

        <section>
            <h2>8. Změny těchto zásad</h2>
            <p>Tyto zásady můžeme občas aktualizovat. O podstatných změnách vás budeme informovat prostřednictvím aplikace nebo emailu. Aktuální verze je vždy dostupná na této stránce.</p>
        </section>

        <div class="contact-box">
            <h2>9. Kontakt</h2>
            <p>Pokud máte dotazy ohledně ochrany vašich údajů, kontaktujte nás:</p>
            <p><a href="mailto:michal.simon.777@gmail.com">michal.simon.777@gmail.com</a></p>
        </div>
    </div>

    <!-- ENGLISH VERSION -->
    <div class="content-section" id="content-en">
        <p class="effective-date">Effective date: March 1, 2026</p>

        <section>
            <h2>1. Introduction</h2>
            <p>FitFactory ("the app") is a mobile application for tracking strength training workouts. Your privacy is important to us. This policy describes what data we collect, how we use it, and how we protect it.</p>
        </section>

        <section>
            <h2>2. Data We Collect</h2>

            <table class="data-table">
                <thead>
                    <tr>
                        <th>Data Type</th>
                        <th>Purpose</th>
                        <th>Storage</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Email and password</td>
                        <td>Registration and login</td>
                        <td>Firebase Authentication (Google Cloud)</td>
                    </tr>
                    <tr>
                        <td>Display name</td>
                        <td>In-app identification</td>
                        <td>Firebase Firestore</td>
                    </tr>
                    <tr>
                        <td>Nickname</td>
                        <td>User search</td>
                        <td>Firebase Firestore</td>
                    </tr>
                    <tr>
                        <td>Profile photo</td>
                        <td>Optional personalization</td>
                        <td>Firebase Storage</td>
                    </tr>
                    <tr>
                        <td>Workout data</td>
                        <td>Progress tracking</td>
                        <td>Locally on device</td>
                    </tr>
                    <tr>
                        <td>Personal records</td>
                        <td>Training weight calculation</td>
                        <td>Locally on device</td>
                    </tr>
                </tbody>
            </table>

            <div class="highlight-box">
                <p><strong>Important:</strong> Your workout data (workouts, sets, weights, personal records) is stored exclusively on your device. It is not sent to our servers unless you choose to use the trainer sharing feature.</p>
            </div>
        </section>

        <section>
            <h2>3. How We Use Your Data</h2>
            <p>We use your data exclusively for:</p>
            <p>• Authentication and account management</p>
            <p>• Communication between trainer and client (if you use this feature)</p>
            <p>• Workout sharing and notifications within the trainer-client system</p>
            <p>• Improving the app based on anonymous aggregated statistics</p>
        </section>

        <section>
            <h2>4. Third-Party Data Sharing</h2>
            <p>We <strong>do not sell or share</strong> your personal data with third parties for advertising or marketing purposes.</p>
            <p>We only share data in the following cases:</p>
            <p>• <strong>Firebase / Google Cloud</strong> – for authentication and cloud services (in accordance with Google Cloud terms)</p>
            <p>• <strong>Trainer-client</strong> – your workout data is shared with a trainer only based on your explicit consent (accepting a connection request)</p>
        </section>

        <section>
            <h2>5. Security</h2>
            <p>All communication between the app and servers is encrypted (HTTPS/TLS). Firebase Authentication ensures secure storage of login credentials. Access to cloud database is governed by Firebase security rules.</p>
        </section>

        <section>
            <h2>6. Your Rights</h2>
            <p>You have the right to:</p>
            <p>• <strong>Access</strong> your data stored in the app</p>
            <p>• <strong>Correct</strong> your personal information in profile settings</p>
            <p>• <strong>Delete</strong> your account and all associated cloud data</p>
            <p>• <strong>Export</strong> your workout data (backup feature)</p>
            <p>Local workout data is deleted when you uninstall the app.</p>
        </section>

        <section>
            <h2>7. Children</h2>
            <p>FitFactory is not intended for children under 16. We do not knowingly collect data from persons under 16 years of age.</p>
        </section>

        <section>
            <h2>8. Changes to This Policy</h2>
            <p>We may update this policy from time to time. We will notify you of significant changes through the app or email. The current version is always available on this page.</p>
        </section>

        <div class="contact-box">
            <h2>9. Contact</h2>
            <p>If you have questions about your data privacy, contact us at:</p>
            <p><a href="mailto:michal.simon.777@gmail.com">michal.simon.777@gmail.com</a></p>
        </div>
    </div>

    <div class="footer">
        &copy; 2026 FitFactory. All rights reserved.
    </div>
</div>

<script>
    function switchLang(lang) {
        document.getElementById('content-cs').classList.toggle('active', lang === 'cs');
        document.getElementById('content-en').classList.toggle('active', lang === 'en');
        document.getElementById('btn-cs').classList.toggle('active', lang === 'cs');
        document.getElementById('btn-en').classList.toggle('active', lang === 'en');
        document.getElementById('page-title').textContent =
            lang === 'cs' ? 'Zásady ochrany osobních údajů' : 'Privacy Policy';
        document.documentElement.lang = lang;
    }
</script>

</body>
</html>
