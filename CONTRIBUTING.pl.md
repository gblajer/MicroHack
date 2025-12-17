# Współtworzenie MicroHacków

Dziękujemy za zainteresowanie naszymi MicroHackami!

- [Współtworzenie MicroHacków](#współtworzenie-microhacków)
- [Jak współtworzyć 🚀](#jak-współtworzyć-)
- [Wytyczne dotyczące współtworzenia 🚩](#wytyczne-dotyczące-współtworzenia-)
- [Cel MicroHack](#cel-microhack)
- [Organizacja repozytorium](#organizacja-repozytorium)
  - [Gałęzie](#gałęzie)
- [Narzędzia do tworzenia](#narzędzia-do-tworzenia)
- [Narzędzia IaC](#narzędzia-iac)
- [Jak używać Markdown do formatowania tematów](#jak-używać-markdown-do-formatowania-tematów)
- [Nazwy plików i folderów](#nazwy-plików-i-folderów)
- [Szablon](#szablon)
- [Formatowanie](#formatowanie)
  - [Nagłówki i nawigacja po prawej stronie](#nagłówki-i-nawigacja-po-prawej-stronie)
  - [Formatowanie tekstu](#formatowanie-tekstu)
  - [Linki](#linki)
  - [Zakładki](#zakładki)
  - [Obrazy](#obrazy)

## Jak współtworzyć 🚀

Aby współtworzyć [MicroHacki](./README.pl.md), musisz sforkować to repozytorium i przesłać pull request z proponowanymi zmianami w plikach Markdown i/lub obrazach.

* [Jak sforkować repozytorium](https://help.github.com/articles/fork-a-repo)
* [Jak utworzyć pull request](https://help.github.com/articles/creating-a-pull-request/)
* [Zmiana wiadomości commit](https://help.github.com/articles/changing-a-commit-message/)
* [Jak scalić commity](https://help.github.com/articles/about-pull-request-merges/)

## Wytyczne dotyczące współtworzenia 🚩

Ten projekt przyjmuje wkłady i sugestie. Większość wkładów wymaga zaakceptowania
Umowy Licencyjnej Współtwórcy (CLA), która deklaruje, że masz prawo i faktycznie
przyznasz nam prawa do korzystania z twojego wkładu. Szczegóły znajdziesz na stronie https://cla.opensource.microsoft.com.

Kiedy wysyłasz pull request, bot CLA automatycznie określi, czy musisz dostarczyć
CLA i odpowiednio ozdobi PR (np. sprawdzenie statusu, komentarz). Po prostu postępuj zgodnie z instrukcjami
dostarczonymi przez bota. Będziesz musiał to zrobić tylko raz we wszystkich repozytoriach korzystających z naszej CLA.

Ten projekt przyjął [Kodeks Postępowania Microsoft Open Source](https://opensource.microsoft.com/codeofconduct/).
Aby uzyskać więcej informacji, zobacz [FAQ Kodeksu Postępowania](https://opensource.microsoft.com/codeofconduct/faq/) lub
skontaktuj się z [opencode@microsoft.com](mailto:opencode@microsoft.com) w przypadku dodatkowych pytań lub komentarzy.

## Cel MicroHack

Proszę zapoznać się z [MicroHack Readme](./README.pl.md)

## Organizacja repozytorium

Zawartość tego repozytorium jest zgodna z różnymi obszarami rozwiązań w Azure i M365.

To repozytorium zawiera następujące foldery:

* \01-Identity and Access Management
* \02-Security
* \03-Azure
* \04-Microsoft-365
* \99-MicroHack-Template

W tych folderach znajdziesz MicroHacki oraz pliki Markdown używane do treści. Każdy z tych folderów zawiera również folder `\images`, który odnosi się do obrazów (takich jak zrzuty ekranu) używanych w MicroHackach. Folder `\iac` zawiera niezbędne pliki wdrożeniowe (ARM, Bicep, Terraform).

### Gałęzie

Zalecamy tworzenie lokalnych gałęzi roboczych, które są ukierunkowane na określony zakres zmian (a następnie przesłanie pull requesta, gdy zmiany są gotowe). Każda gałąź powinna być ograniczona do pojedynczego MicroHacka, zarówno w celu usprawnienia przepływu pracy, jak i zmniejszenia możliwości konfliktów scalania. Następujące działania są odpowiednim zakresem dla nowej gałęzi:

* Nowy temat (i powiązane obrazy).
* Poprawki ortograficzne i gramatyczne w temacie.
* Zastosowanie pojedynczej zmiany formatowania w dużym zestawie tematów.

## Nazwy plików i folderów

Używaj małych liter dla nazw plików i folderów oraz myślników `-` jako separatorów.

Na przykład:

* `/01-identity-and-access-management/01-zero-trust/readme.md`
* `/01-identity-and-access-management/02-azure-ad-pim/readme.md`
* `/02-azure/01-infrastructure/01-azure-virtual-desktop/readme.md`
* `/02-azure/02-data/01-azure-sql-mi/readme.md`
* `/03-microsoft365/01-exchange-online/readme.md`

## Jak używać Markdown do formatowania tematów

Tematy w tym repozytorium używają Markdown. Oto dobry przegląd [podstaw Markdown](https://help.github.com/articles/markdown-basics/).

## Narzędzia do tworzenia

[Visual Studio Code](https://code.visualstudio.com) to świetny edytor dla Markdown!

## Narzędzia IaC

W przypadku, gdy musisz wdrożyć usługi Azure jako warunek wstępny dla MicroHacka, użyj znanych rozwiązań, takich jak szablony ARM, Bicep lub Terraform lub Azure CLI.
Proszę również dołączyć instrukcje wdrożenia w swoim przewodniku.

## Szablony
### Nowy MicroHack

W celu szybkiego rozpoczęcia nowych MicroHacków stworzyliśmy [szablon](99-MicroHack-Template/Readme.md) dla twojej wygody. Proszę użyć tego szablonu, aby upewnić się, że twój microhack pasuje do struktury obecnych microhacków. Mile widziane są również wkłady/ulepszenia szablonu.
Aby rozpocząć nowy MicroHack, utwórz odpowiedni issue [tutaj](https://github.com/microsoft/MicroHack/issues).

### Połączony MicroHack

Zdajemy sobie sprawę, że format MicroHack nie jest ekskluzywny dla tego repozytorium. Aby dać ci szansę na promowanie swojego MicroHacka i ułatwić jego odkrycie, możesz użyć [szablonu linku](99-MicroHack-TemplateLink/Readme.md), aby połączyć swój MicroHack.

## Formatowanie

### Nagłówki i nawigacja po prawej stronie

Podtytuły H2 `##` kończą się na liście przejść po prawej stronie dla dokumentu (lista przejść jest tworzona przez nasz skrypt kompilacji). Dobrym pomysłem jest dołączenie podtytułów h2, aby pomóc użytkownikom uzyskać przegląd dokumentu i szybko nawigować do głównych tematów.

### Linki

Dla linków w naszym własnym repozytorium użyj linku względnego do witryny, takiego jak `/readme.md`.

>Na przykład: `[Kodeks Postępowania](/CODE_OF_CONDUCT.md)` - łączy do strony **Kodeksu Postępowania**

>**Uwaga:** Dla nawigacji na GitHub, powinieneś dodać rozszerzenie .md.

### Zakładki

Aby zapewnić linki do podtytułów h2 (Markdown ##), format to `[Tekst linku](tytuł-podtytułu)`.

Zwróć uwagę, że tytuł podtytułu jest małymi literami, a słowa tytułu podtytułu są oddzielone myślnikami `-`.

### Obrazy

Obrazy są ważne, aby ożywić MicroHack i wyjaśnić pisaną treść.

Dla obrazów, które dodajesz do repozytorium, przechowuj je w podfolderze `images` sekcji MicroHack, na przykład:
`01-identity-and-access-management/01-zero-trust/images/`

Kiedy linkujesz do obrazu, ścieżka i nazwa pliku są wrażliwe na wielkość liter. Konwencją jest, aby nazwy plików obrazów były małymi literami i używały myślników `-` jako separatorów.

>Na przykład: `![Zrzut ekranu](images/step1-create-vm.png)`

### Alerty

Proszę używać domyślnych opcji GitHub do podkreślenia krytycznych informacji

```
> [!NOTE]
> Podkreśla informacje, które użytkownicy powinni wziąć pod uwagę, nawet podczas przeglądania.

> [!IMPORTANT]
> Kluczowe informacje niezbędne dla użytkowników do osiągnięcia sukcesu.

> [!WARNING]
> Krytyczna treść wymagająca natychmiastowej uwagi użytkownika ze względu na potencjalne ryzyko.
```
Co spowoduje świetną wizualizację:
> [!NOTE]
> Podkreśla informacje, które użytkownicy powinni wziąć pod uwagę, nawet podczas przeglądania.

> [!IMPORTANT]
> Kluczowe informacje niezbędne dla użytkowników do osiągnięcia sukcesu.

> [!WARNING]
> Krytyczna treść wymagająca natychmiastowej uwagi użytkownika ze względu na potencjalne ryzyko.
