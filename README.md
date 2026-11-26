# Vorleser auf Pages · Testlabor

Testseite für die Live-Verbindung zwischen GitHub Pages und der internen Claude-App „Pages-Brücke“.

- Die Seite wird von der Pages-Brücke als Fenster geöffnet und tauscht mit ihr Nachrichten aus (`postMessage`, Format `vlp` Version 1).
- Sprachmodell- und Connector-Aufrufe (Canva, Hugging Face) macht die App; Pollinations lädt die Seite direkt.
- Alle Inhalte im Repository liegen nur verschlüsselt vor (AES-GCM 256, PBKDF2-SHA256 mit 310 000 Durchläufen, gezippt) – dasselbe Verfahren wie im Vorleser. Das Passwort liegt nie im Repository.
