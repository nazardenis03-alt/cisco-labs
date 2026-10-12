# Cisco Router Hardening & SSH Security Lab

Projekt przedstawiający konfigurację bezpiecznego dostępu zdalnego oraz podstawowe mechanizmy twardnienia (Device Hardening) urządzeń sieciowych Cisco zgodnie z dobrymi praktykami cyberbezpieczeństwa.

## 🔒 Zastosowane mechanizmy bezpieczeństwa
* **Szyfrowany dostęp zdalny (SSH v2):** Całkowite wyłączenie przestarzałego i nieszyfrowanego protokołu Telnet na liniach VTY (`transport input ssh`).
* **Kryptografia:** Generowanie 1024-bitowych kluczy RSA oraz wymóg konfiguracji nazwy domeny.
* **Ochrona przed Brute-Force:** Automatyczna blokada dostępu po 3 nieudanych próbach logowania na 60 sekund (`login block-for 60 attempts 3 within 30`).
* **Zarządzanie hasłami:** Szyfrowanie wszystkich haseł w pliku konfiguracyjnym (`service password-encryption`) oraz mocne hasło dla trybu uprzywilejowanego (`enable secret`).
* **Bezpieczeństwo sesji:** Automatyczne wylogowanie z konsoli i linii VTY po określonym czasie bezczynności (timeout).

## 📁 Zawartość repozytorium
* `Cisco_Router_Security_Lab.pkt` – Plik projektu wykonany w Cisco Packet Tracer.
