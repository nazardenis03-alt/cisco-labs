# Cisco Packet Tracer - Secure VLAN & Inter-VLAN Routing Lab

Projekt laboratorium sieciowego przedstawiający konfigurację segmentacji ruchu, routingu między-sieciowego oraz podstawowych reguł kontroli dostępu (ACL) ze względów bezpieczeństwa.

## 🛠️ Architektura i Konfiguracja
* **Segmentacja VLAN:** 
  * VLAN 10 (`OFFICE`) - Sieć biurowa
  * VLAN 20 (`GUEST`) - Sieć dla gości (ograniczony dostęp)
  * VLAN 30 (`SERVERS`) - Sieć serwerowa
* **Switching:** Konfiguracja portów dostępowych (Access) oraz portu trunkingowego (Trunk) łączącego switch z routerem.
* **Routing:** Inter-VLAN routing zrealizowany na routerze przy użyciu subinterfejsów i enkapsulacji IEEE 802.1Q.
* **Bezpieczeństwo (ACL):** Zaimplementowana rozszerzona lista kontroli dostępu (`BLOKUJ_GOSCIA`), która blokuje ruch z sieci gości (VLAN 20) do serwerów (VLAN 30), pozwalając jednocześnie na pozostałą komunikację.

## 📁 Zawartość repozytorium
* `network_lab.pkt` – Plik projektu Cisco Packet Tracer.
