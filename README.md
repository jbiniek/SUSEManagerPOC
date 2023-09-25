# SUSEManagerPOC
Informacje pomocnicze do Proof of Concept SUSE Managera

## Instalacja serwera SUSE Manager

### Wymagania sprzętowe
- 4vCPU
- 8GB RAM (zalecane 16GB)
- Rozszerzalna przestrzeń dyskowa (LVM) 500GB minimum, zalecane 1TB

### Wymagania sieciowe
- Dostępna pełna nazwa domenowa dla serwera (FQDN)
- DNS, który poprawnie rozwiązuje nazwy zarówno serwera, jak i klientów
- Otwarte porty przychodzące (minimum): 22, 80, 443, 4505, 4506
- Otwarte porty wychodzące (minimum): 80, 443
- Adres scc.suse.com oraz updates.suse.com dostępny z serwera

Pełna dokumentacja dotycząca przygotowania oraz instalacji: https://documentation.suse.com/suma/4.3/en/suse-manager/installation-and-upgrade/installation-and-upgrade-overview.html

### Integracja z VMWare (opcjonalnie)
Potrzebne będzie konto serwisowe hosta VMWare, które posiada uprawnienia przynajmniej read-only do obiektów, które mają być widoczne dla SUSE Managera (zazwyczaj wszystkie). Najlepiej przygotować też od razu pełny adres FQDN (ew. IP) hosta, upewnić się jakiego portu używa API VMWare (np. 443), oraz naturalnie przygotować nazwę i hasło konta które chcemy przekazać do SUSE Managera.
