<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover">
<title>GNSS Max Privacy Policy</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Instrument+Sans:wght@400;500;600;700&family=JetBrains+Mono:wght@500&display=swap">
<style>
/* Layout: single reading column, instrument-panel header strip, data-flow table as the one "set-off" element */
:root{
  --bg:#f6f8f7; --surface:#ffffff; --fg:#141a17; --muted:#5b6862; --line:#dbe3df; --accent:#16804f; --accent-soft:#e3f3ea;
  --f-body:'Instrument Sans',system-ui,-apple-system,'Segoe UI',sans-serif;
  --f-mono:'JetBrains Mono',ui-monospace,Consolas,monospace;
}
@media (prefers-color-scheme: dark){:root:not([data-theme="light"]){
  --bg:#0d0f13; --surface:#151a20; --fg:#e4ebe7; --muted:#8f9c95; --line:#252d34; --accent:#6ad396; --accent-soft:#163024; color-scheme:dark}}
:root[data-theme="dark"]{
  --bg:#0d0f13; --surface:#151a20; --fg:#e4ebe7; --muted:#8f9c95; --line:#252d34; --accent:#6ad396; --accent-soft:#163024; color-scheme:dark}

body{background:var(--bg);color:var(--fg);font:16px/1.65 var(--f-body);
  padding-left:max(16px,env(safe-area-inset-left,0px));padding-right:max(16px,env(safe-area-inset-right,0px));padding-block:0 64px}
main{max-width:44rem;margin:0 auto}
header{padding-block:48px 28px;border-bottom:1px solid var(--line);display:grid;gap:10px}
.eyebrow{font:500 12px/1 var(--f-mono);letter-spacing:.12em;text-transform:uppercase;color:var(--accent)}
h1{margin:0;font-size:clamp(30px,6vw,42px);line-height:1.1;font-weight:700;letter-spacing:-.02em;text-wrap:balance}
.meta{color:var(--muted);font-size:14px;display:flex;flex-wrap:wrap;gap:4px 18px}
.meta span{font-family:var(--f-mono);font-size:12.5px}
.summary{margin-top:28px;padding:18px 20px;border-radius:12px;background:var(--accent-soft);color:var(--fg)}
.summary strong{color:var(--accent)}
h2{margin:40px 0 8px;font-size:20px;line-height:1.3;font-weight:600;text-wrap:balance}
p,li{max-width:65ch}
p{margin:0 0 12px}
ul{margin:0 0 12px;padding-left:1.2em;display:grid;gap:6px}
a{color:var(--accent);text-underline-offset:3px}
a:focus-visible{outline:2px solid var(--accent);outline-offset:2px;border-radius:2px}
code{font:500 13.5px var(--f-mono);background:var(--surface);border:1px solid var(--line);padding:1px 5px;border-radius:5px}
.tablewrap{overflow-x:auto;margin:12px 0 4px;border:1px solid var(--line);border-radius:12px;background:var(--surface)}
table{border-collapse:collapse;width:100%;min-width:560px;font-size:14.5px}
th,td{text-align:left;vertical-align:top;padding:11px 14px;border-bottom:1px solid var(--line)}
tr:last-child td{border-bottom:0}
th{font:500 11.5px/1.3 var(--f-mono);letter-spacing:.08em;text-transform:uppercase;color:var(--muted)}
td:first-child{font-weight:600;white-space:nowrap}
.contact{display:flex;flex-wrap:wrap;align-items:center;gap:10px}
.contact span{font-family:var(--f-mono);font-size:14px;user-select:all}
button{font:500 13px var(--f-body);color:var(--accent);background:transparent;border:1px solid var(--line);border-radius:8px;padding:4px 10px;cursor:pointer}
button:focus-visible{outline:2px solid var(--accent);outline-offset:2px}
footer{margin-top:44px;padding-top:18px;border-top:1px solid var(--line);color:var(--muted);font-size:14px}
</style>
</head>
<body>

<main>
  <header>
    <div class="eyebrow">GNSS Max · iOS</div>
    <h1>Privacy Policy</h1>
    <div class="meta">Effective <span>29 October 2026</span> Developer <span>Petr Novotný</span></div>
  </header>

  <div class="summary"><strong>In short:</strong> GNSS Max does not collect, store or share your personal data on any server. There is no account, no analytics, no advertising and no tracking. Your location is processed on your iPhone. It is only sent to third-party services when you use a feature that needs it, and only to that service.</div>

  <h2>Who is responsible</h2>
  <p>GNSS Max is developed and published by Petr Novotný, an individual developer based in the Czech Republic. For any privacy question, see <a href="#contact">Contact</a> below.</p>

  <h2>Data the app uses on your device</h2>
  <ul>
    <li><strong>Location.</strong> GNSS Max uses your position to display coordinates, altitude, speed and accuracy, to record tracks and to compute satellite and Sun/Moon positions. With the "Always" permission it can keep recording a track in the background while a recording is running. You can change or revoke location access at any time in iOS Settings.</li>
    <li><strong>Motion and fitness (barometer).</strong> Air pressure is read to compute barometric altitude.</li>
    <li><strong>Local network.</strong> Used only when you connect to an external GNSS receiver on your Wi-Fi (NMEA over TCP). Data from the receiver stays on your device.</li>
    <li><strong>Stored on your device.</strong> Recorded tracks, saved points, app settings and downloaded satellite orbital elements are stored in the app's local storage. The NTRIP password is stored in the iOS Keychain. The Home Screen widget and Live Activity read your latest position from a storage area shared only with the app's own widget.</li>
  </ul>
  <p>None of this data is sent to the developer. Deleting the app deletes all of it.</p>

  <h2>When data leaves your device</h2>
  <p>Some features contact a third-party service. Each request goes directly from your iPhone to that service and only happens when you use the feature.</p>
  <div class="tablewrap">
    <table>
      <thead><tr><th>Feature</th><th>Service</th><th>What is sent</th></tr></thead>
      <tbody>
        <tr><td>Address of your position</td><td>Apple (reverse geocoding)</td><td>Your coordinates, to look up the place name shown on the dashboard</td></tr>
        <tr><td>Map</td><td>Apple Maps</td><td>Map tile requests for the area you view</td></tr>
        <tr><td>METAR / QNH</td><td>aviationweather.gov (NOAA, USA)</td><td>An approximate area around your position, to find the nearest airport report</td></tr>
        <tr><td>Satellite prediction</td><td>CelesTrak</td><td>A download request for orbital elements; no location is sent</td></tr>
        <tr><td>NTRIP corrections</td><td>The caster you configure (e.g. CZEPOS)</td><td>Your user name and password for that caster and, for network corrections, your approximate position (an NMEA GGA sentence every 10 s)</td></tr>
        <tr><td>External receiver</td><td>A device on your local network</td><td>Correction data you choose to forward; nothing leaves your network</td></tr>
      </tbody>
    </table>
  </div>
  <p>These services handle requests under their own privacy policies. GNSS Max adds no identifiers to these requests and does not combine their results with any other data.</p>

  <h2>Exported data</h2>
  <p>When you export a track as GPX or share an NMEA log, the file goes wherever you send it through the iOS share sheet. What happens to it after that is up to you and the app you share it with.</p>

  <h2>What GNSS Max does not do</h2>
  <ul>
    <li>No user accounts or sign-in</li>
    <li>No analytics, crash-reporting or advertising SDKs</li>
    <li>No tracking across apps or websites, and no sale of data</li>
    <li>No collection of contacts, photos, health data or identifiers</li>
  </ul>

  <h2>Children</h2>
  <p>GNSS Max is a general-purpose utility and is not directed at children. It collects no personal data from anyone.</p>

  <h2>Your rights</h2>
  <p>Because the developer holds no personal data about you, there is nothing to access, correct or delete on our side. You control everything stored by the app on your device, and you can remove it by deleting tracks and points in the app or by deleting the app. Under the GDPR you may still contact the developer or lodge a complaint with your data protection authority (in the Czech Republic: ÚOOÚ, <a href="https://uoou.gov.cz" target="_blank" rel="noopener">uoou.gov.cz</a>).</p>

  <h2>Changes</h2>
  <p>If the app's data handling changes, this policy will be updated and the effective date above will change.</p>

  <h2 id="contact">Contact</h2>
  <div class="contact"><span id="mail">mischwitz@gmail.com</span><button id="copy" type="button">Copy</button></div>

  <footer>GNSS Max is not certified for aviation navigation. Accuracy depends on your device, sky visibility and environment.</footer>
</main>

<script>
document.getElementById('copy').addEventListener('click', async e => {
  const b = e.currentTarget, t = document.getElementById('mail').textContent;
  try { await navigator.clipboard.writeText(t); b.textContent = 'Copied'; }
  catch { const r = document.createRange(); r.selectNodeContents(document.getElementById('mail'));
          const s = getSelection(); s.removeAllRanges(); s.addRange(r); b.textContent = 'Selected'; }
  setTimeout(() => b.textContent = 'Copy', 1800);
});
</script>
</body>
</html>
