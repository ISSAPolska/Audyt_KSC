# Metodyka przeprowadzania audytu zgodnego z KSC

## Spis treści

[Historia zmian 3]()

[Podziękowania 3]()

[Skróty i definicje 4]()

[Wprowadzenie 4]()

[Podstawowe zasady przeprowadzania audytów bezpieczeństwa informacji 5]()

[Zasada niezależności 5]()

[Zasada obiektywności 5]()

[Zasada zachowania poufności 5]()

[Zasada należytych kompetencji 5]()

[Zasada kompletności prac 5]()

[Zasada weryfikacji poprawności zaprojektowania mechanizmu kontrolnego 6]()

[Zasada próbkowania 6]()

[Metodyka audytu zgodności z KSC \(na razie bez rozp.\) 7]()

[Planowanie prac 7]()

[Etap I – Analiza Dokumentacji 7]()

[Analiza zapisów 9]()

[Etap II – Testy skuteczności funkcjonowania mechanizmów kontrolnych 10]()

[Raportowanie 10]()

## Historia zmian

| Data | Wersja | Imię i Nazwisko | Zakres zmian |
| :--- | :--- | :--- | :--- |
|  |  |  |  |

## Skróty i definicje

<table>
  <thead>
    <tr>
      <th style="text-align:left">Definicja</th>
      <th style="text-align:left">Wyja&#x15B;nienie</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">
        <p></p>
        <p>Audytor Wiod&#x105;cy</p>
      </td>
      <td style="text-align:left">Audytor wyznaczony jako lider zespo&#x142;u audytowego, odpowiedzialny
        za zakres audytu, jego programu, wyb&#xF3;r technik badawczych oraz przygotowanie
        zbiorczego raportu</td>
    </tr>
    <tr>
      <td style="text-align:left">Common Vulnerability Scoring System (CVSS)</td>
      <td style="text-align:left">Mi&#x119;dzynarodowa skala stosowana podczas analizy ryzyk zwi&#x105;zanych
        z technicznymi podatno&#x15B;ciami system&#xF3;w informatycznych. Jest
        stosowana przez wszystkich g&#x142;&#xF3;wnych dostawc&#xF3;w system&#xF3;w
        informatycznych oraz powszechnie wykorzystywana na ca&#x142;ym &#x15B;wiecie
        przez zespo&#x142;y IT. Jest szerzej opisana na stronie https://www.first.org/cvss/</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p></p>
        <p>KSC</p>
      </td>
      <td style="text-align:left">
        <p></p>
        <p>Ustawa o Krajowym Systemie Cyberbezpiecze&#x144;stwa</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">OUK</td>
      <td style="text-align:left">Operator Us&#x142;ugi Kluczowej</td>
    </tr>
    <tr>
      <td style="text-align:left">UK</td>
      <td style="text-align:left">Us&#x142;uga Kluczowa - zestaw funkcji, towar&#xF3;w i us&#x142;ug uznanych
        przez Organ W&#x142;a&#x15B;ciwych za istotny dla sprawnego dzia&#x142;ania
        Cyberbezpiecze&#x144;stwa Rzeczypospolitej Polskiej</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p></p>
        <p>Mechanizm kontrolny</p>
      </td>
      <td style="text-align:left">&#x15B;rodk&#xF3;w technicznych i organizacyjnych (fizyczne i informatyczne
        narz&#x119;dzia, procedury operacyjne i instrukcje oraz struktura organizacyjna)
        maj&#x105;ce na celu zmniejszanie zidentyfikowanego ryzyka. Jest to to&#x17C;same
        z terminem &#x201E;zabezpieczenie&#x201D;</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p></p>
        <p>Najwy&#x17C;sze Kierownictwo</p>
      </td>
      <td style="text-align:left">osoba lub grupa os&#xF3;b, kt&#xF3;re na najwy&#x17C;szym szczeblu kieruj&#x105;
        organizacj&#x105; i j&#x105; nadzoruj&#x105;</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p></p>
        <p>Program audytu</p>
      </td>
      <td style="text-align:left">przygotowany przez Audytora Wiod&#x105;cego i zatwierdzony przez Operatora
        Us&#x142;ugi Kluczowej program zadania audytowego</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p></p>
        <p>Raport z audytu</p>
      </td>
      <td style="text-align:left">dokument przygotowany pod nadzorem Audytora Wiod&#x105;cego zawieraj&#x105;cy
        obserwacje (ustalenia stanu faktycznego) w zakresie zaobserwowanych niezgodno&#x15B;ci,
        ocen&#x119; systemu, klasyfikacj&#x119; zidentyfikowanego ryzyka oraz rekomendacje
        dla Kierownictwa OUK</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p></p>
        <p>Skuteczno&#x15B;&#x107; mechanizmu kontrolnego</p>
      </td>
      <td style="text-align:left">zapewnienie, &#x17C;e mechanizm kontrolny realizuje postawione przed nim
        cele</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p></p>
        <p>Zesp&#xF3;&#x142; audytowy</p>
      </td>
      <td style="text-align:left">
        <p></p>
        <p>Audytor Wiod&#x105;cy oraz co najmniej jeden dodatkowy audytor przeprowadzaj&#x105;cy
          zadanie audytowe</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p></p>
        <p>System informatyczny</p>
      </td>
      <td style="text-align:left">system informatyczny wykorzystywany do &#x15B;wiadczenia us&#x142;ugi
        kluczowej</td>
    </tr>
    <tr>
      <td style="text-align:left">Operator us&#x142;ugi kluczowej</td>
      <td style="text-align:left">Podmiot gospodarczy wykonuj&#x105;cy dzia&#x142;ania uznane przez pa&#x144;stwo
        Polskie za istotne, a wobec kt&#xF3;rego organ w&#x142;a&#x15B;ciwy do
        spraw cyberbezpiecze&#x144;stwa wyda&#x142; decyzj&#x119; o uznaniu za
        operatora us&#x142;ugi kluczowej</td>
    </tr>
    <tr>
      <td style="text-align:left">Organ w&#x142;a&#x15B;ciwy</td>
      <td style="text-align:left">Organami w&#x142;a&#x15B;ciwymi do spraw cyberbezpiecze&#x144;stwa s&#x105;
        ministerowie w&#x142;a&#x15B;ciwi do spraw zgodnie z podzia&#x142;em sektorowym.
        Organ w&#x142;a&#x15B;ciwy kontroluje i nak&#x142;ada kary pieni&#x119;&#x17C;ne
        na operator&#xF3;w us&#x142;ug kluczowych i dostawc&#xF3;w us&#x142;ug
        cyfrowych</td>
    </tr>
    <tr>
      <td style="text-align:left">zarz&#x105;dzanie incydentem</td>
      <td style="text-align:left">
        <p>bie&#x17C;&#x105;cy i udokumentowany proces og&#xF3;lnego post&#x119;powania
          w trakcie obs&#x142;ugi incydentu polegaj&#x105;cego conajmniej na podejmowaniu
          dzia&#x142;a&#x144; i dokumentowania z podzia&#x142;em na fazy:</p>
        <ul>
          <li>wyszukiwanie powi&#x105;za&#x144; mi&#x119;dzy incydentami,</li>
          <li>usuwanie przyczyn ich wyst&#x105;pienia</li>
          <li>opracowywanie wniosk&#xF3;w</li>
        </ul>
        <p>wynikaj&#x105;cych z obs&#x142;ugi incydentu</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">szacowanie ryzyka</td>
      <td style="text-align:left">
        <p>bie&#x17C;&#x105;ce prace polegaj&#x105;ce na ocenie sytuacji w zarz&#x105;dzanej
          cyberprzestrzeni polegaj&#x105;ce co najmniej na:</p>
        <p></p>
        <ul>
          <li>identyfikacji</li>
          <li>analizie</li>
          <li>ocenie ryzyka</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">obs&#x142;uga incydentu</td>
      <td style="text-align:left">
        <p>szczeg&#xF3;&#x142;owy zestaw czynno&#x15B;ci wykonywanych w spos&#xF3;b
          powtarzalny i udokumentowany, a sk&#x142;adaj&#x105;cy si&#x119; z co najmniej
          faz:</p>
        <p></p>
        <ul>
          <li>wykrywanie</li>
          <li>rejestrowanie</li>
          <li>analizowanie</li>
          <li>klasyfikowanie</li>
          <li>priorytetyzacj&#x119;</li>
          <li>podejmowanie dzia&#x142;a&#x144; naprawczych</li>
          <li>ograniczenie skutk&#xF3;w incydentu</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Pe&#x142;nomocnik OUK</td>
      <td style="text-align:left">osoba odpowiedzialn&#x105; za utrzymywanie kontakt&#xF3;w z podmiotami
        krajowego systemu cyberbezpiecze&#x144;stwa</td>
    </tr>
    <tr>
      <td style="text-align:left">W&#x142;a&#x15B;ciciel procesu zarz&#x105;dzania ryzykiem</td>
      <td style="text-align:left">Osoba odpowiedzialna u OUK za wype&#x142;nianie obowi&#x105;zk&#xF3;w
        operatora w zakresie artyku&#x142;u 8 punkt 1.</td>
    </tr>
    <tr>
      <td style="text-align:left">W&#x142;a&#x15B;ciciel procesu zarz&#x105;dzania incydentem</td>
      <td style="text-align:left">Osoba odpowiedzialna u OUK za wype&#x142;nianie obowi&#x105;zk&#xF3;w
        operatora w zakresie artyku&#x142;u 8 punkt 4</td>
    </tr>
    <tr>
      <td style="text-align:left">W&#x142;a&#x15B;ciciel procesu zarz&#x105;dzania zagro&#x17C;eniami</td>
      <td
      style="text-align:left">Osoba odpowiedzialna u OUK za wype&#x142;nianie obowi&#x105;zk&#xF3;w
        operatora w zakresie artyku&#x142;u 8 punkt 3 w zakresie zbieranie informacji
        o zagro&#x17C;eniach cyberbezpiecze&#x144;stwa dla systemu informacyjnego
        wykorzystywanego do &#x15B;wiadczenia us&#x142;ugi kluczowej.</td>
    </tr>
    <tr>
      <td style="text-align:left">W&#x142;a&#x15B;ciciel procesu zarz&#x105;dzania podatno&#x15B;ciami</td>
      <td
      style="text-align:left">Osoba odpowiedzialna u OUK za wype&#x142;nianie obowi&#x105;zk&#xF3;w
        operatora w zakresie artyku&#x142;u 8 punkt 3 w zakresie identyfikacji
        i post&#x119;powania z podatno&#x15B;ciami na incydenty systemu informacyjnego
        wykorzystywanego do &#x15B;wiadczenia us&#x142;ugi kluczowej.</td>
    </tr>
    <tr>
      <td style="text-align:left">W&#x142;a&#x15B;ciciel procesu zarz&#x105;dzanie &#x15B;rodkami technicznymi</td>
      <td
      style="text-align:left">Osoba odpowiedzialna u OUK za wype&#x142;nianie obowi&#x105;zk&#xF3;w
        operatora w zakresie artyku&#x142;u 8 punkt 2 w zakresie wdro&#x17C;enie
        odpowiednich i proporcjonalnych do oszacowanego ryzyka &#x15B;rodk&#xF3;w
        technicznych uwzgl&#x119;dniaj&#x105;cych najnowszy stan wiedz zabezpieczaj&#x105;cych
        systemy informacyjne wykorzystywanego do &#x15B;wiadczenia us&#x142;ugi
        kluczowej.</td>
    </tr>
    <tr>
      <td style="text-align:left">W&#x142;a&#x15B;ciciel procesu zarz&#x105;dzanie &#x15B;rodkami organizacyjnymi</td>
      <td
      style="text-align:left">Osoba odpowiedzialna u OUK za wype&#x142;nianie obowi&#x105;zk&#xF3;w
        operatora w zakresie artyku&#x142;u 8 punkt 2 w zakresie wdro&#x17C;enie
        odpowiednich i proporcjonalnych do oszacowanego ryzyka &#x15B;rodk&#xF3;w
        organizacyjnych uwzgl&#x119;dniaj&#x105;cych najnowszy stan wiedz zabezpieczaj&#x105;cych
        systemy informacyjne wykorzystywanego do &#x15B;wiadczenia us&#x142;ugi
        kluczowej.</td>
    </tr>
    <tr>
      <td style="text-align:left">SI_OUK</td>
      <td style="text-align:left">system informacyjny operatora us&#x142;ugi kluczowej identyfikowany w
        organizacji jako jeden lub wiele komponent&#xF3;w technologicznych potrzebnych
        do poprawnego i optymalnego z punktu widzenia ekonomicznego dzia&#x142;ania
        zestawu us&#x142;ug / produkt&#xF3;w uznanych przez organ w&#x142;a&#x15B;ciwy
        za podstaw&#x119; dzia&#x142;ania us&#x142;ugi kluczowej</td>
    </tr>
  </tbody>
</table>## Wprowadzenie

KSC ma na celu ….

Operator usługi kluczowej ma obowiązek zapewnić przeprowadzenie, co najmniej raz na 2 lata, audytu bezpieczeństwa systemu informacyjnego wykorzystywanego do świadczenia usługi kluczowej, zwanego dalej „audytem”. \(art 15\)

Niniejszy dokument ma na celu….

## Podstawowe zasady przeprowadzania audytów bezpieczeństwa informacji

Aby zadanie audytowe w zakresie zgodności OUK z KSC było przeprowadzone w sposób rzetelny należy zapewnić by w jego trakcie przestrzegano szeregu zasad. Te najlepsze praktyki są uznawane przez międzynarodowe organizacje zajmujące się audytem \(np. ISACA - International Information Systems Audit and Control Association oraz IIA - Institute of Internal Auditors\) i często mają poparcie w kodeksach etyki, które obowiązują ich certyfikowanych członków.

Poniżej przedstawiamy kilka z kluczowych zasad prowadzenia audytów zgodności z OUK koniecznych dla spełnienia przed wszystkie osoby przeprowadzające audyt, nie tylko będących certyfikowanymi przez różne organizacje branżowe.

### Zasada niezależności

Zasada niezależności wymaga tego by osoba przeprowadzająca badanie nie była osobą, która wcześniej wykonywała bądź nadzorowała badane zjawiska.

Dodatkowo istotne jest zapewnienie niezależności prac samego zespołu audytowego. Kierownictwo OUK ani inne osoby nie powinny wywierać żadnego wpływu na kształt raportu zawierającego wnioski powstałe w wyniku zadania audytowego.

### Zasada obiektywności

Zespół audytowy powinien zgromadzić obiektywne dowody dla wszystkich stwierdzeń, wniosków i rekomendacji w raporcie audytowym. Dokumentacja powinna być prowadzona w taki sposób, by możliwe było odtworzenie na jakiej podstawie zespół audytowy wysnuł wnioski zapisane w raporcie.

### Zasada zachowania poufności

Audytor jest obowiązany do zachowania w tajemnicy informacji uzyskanych w związku z przeprowadzanym audytem, z zachowaniem przepisów o ochronie informacji niejawnych i innych informacji prawnie chronionych. Zespół audytowy powinien dodatkowo dochować staranności we właściwym zabezpieczeniu wszelkiej dokumentacji zgromadzonej w czasie audytu przez okres zgodny w ustalonymi wymaganiami.

### Zasada należytych kompetencji

Każdy członek zespołu audytowego powinien mieć kompetencje pozwalające na obiektywne zbadanie ustalonego w Programie audytu zakresu prac. W przypadku braku niezbędnych kompetencji Audytor Wiodący może rozszerzyć skład zespołu, przy uwzględnieniu wymagań organizacji, którą reprezentuje oraz wymagań badanego OUK. Nie może być akceptowalny fakt, iż członkowie zespołu audytowego nie posiadają udokumentowanego doświadczenia, kompetencji i kwalifikacji w zakresie oceny obszarów cyberbezpieczeństwa. Obszar cyberbezpieczeństwa można zdefiniować, jako zapewnienie bezpieczeństwa informacji, w tym danych przetwarzanych w środowisku cyfrowym, z wykorzystaniem technologii przesyłu i przetwarzania danych. Brak doświadczenia, kompetencji i kwalifikacji w obszarze technologii teleinformatycznych powinien być traktowany, jako brak należytych kompetencji audytowych obszaru cyberbezpieczeństwa.

### Zasada weryfikacji poprawności zaprojektowania mechanizmu kontrolnego

Badając mechanizmy kontrolne należy w pierwszej kolejności zapewnić, że zostały one zaprojektowane w sposób zapewniający realizację celów, czyli skutecznie zmniejszających zidentyfikowane ryzyko. Dopiero w dalszym kroku należy potwierdzić poprawność wdrożenia danego mechanizmu kontrolnego. Skuteczność przygotowanych rozwiązań należy zweryfikować w trakcie testów.

### Zasada próbkowania

Audyt bazuje na racjonalnym zapewnieniu, które wynika z zakresu nie zawsze obejmującego 100% badanej populacji. Do określenia racjonalnego zapewnienia stosuję się metody próbkowania: statystyczne i niestatystyczne dające badanej stronie zapewnienie, iż badana próba odzwierciedla rzeczywistą populację. Zespół audytowy, na podstawie prac Etapu I szacuje wielkość próby potrzebnej do wykonania zadania audytowego. W realizacji testów należy wyróżnić:

* testy istnienia - weryfikujące istnienie danego mechanizmu kontrolnego;
* testy rzeczywiste - weryfikujące skuteczność działania mechanizmu kontrolnego.

## Komponenty architektoniczne SI\_KSC

### Zgodność dokumentacji systemu z analizą konfiguracji 

Ocenia Sposób przechowania dokumentacji

## Analiza podstawowych procesów

### Szacowanie ryzyka w zakresie wystąpienia incydentu

#### Podstawa prawna

Komponenty architektoniczne SI\_KSC

Akceptowalny poziom ryzyka



metodyki szacowania ryzykiem **wystąpienia incydentu** \(8.1 oraz 10.1\)

## Metodyka audytu zgodności z KSC \(na razie bez rozp.\)

KSC nakłada na OUK obowiązek przeprowadzania audytów w cyklu nie rzadszym niż 2-letni \(art 15.1\). Uwzględniając szczegółowe wymagania organizacji przeprowadzającej audyt oraz badanego podmiotu możliwe ustalenie cyklu dedykowanych audytów częściowych, istotne jest jednakże by w okresie wymaganym KSC zbadane skuteczność wszystkich procesów wchodzących w badany zakres.

Dobrze przeprowadzone zadanie audytowe powinno być wykonane w sposób zapewniający jego powtarzalność w wszystkie zgromadzone dowody audytowe powinny prowadzić do obiektywnych wniosków.

Zespół audytowy powinien składać się co najmniej z dwóch osób spełniających wymagania określone w Art 15 ust. 2.2 i 2.3

Każde zadanie audytowe powinno swym zakresem pokrywać wszystkie odpowiednie wymagania KSC, powinno być wykonane przez kompetentny zespół, zgodnie z zaproponowaną metodyką a wnioski powinny być wdrożone przez Najwyższe Kierownictwo badanego podmiotu w czasie uzgodnionym podczas przyjmowania raportu z audytu.

Za prawidłowe określenie zakresu audytu, jego program, przyjęte techniki badawcze oraz przygotowanie zbiorczego raportu odpowiada Audytor Wiodący danego zadania audytowego.

Każdy członek zespołu audytowego jest obowiązany do zachowania w tajemnicy informacji uzyskanych w związku z przeprowadzanym audytem, z zachowaniem przepisów o ochronie informacji niejawnych i innych informacji prawnie chronionych. Zespół audytowy powinien przeprowadzać prace stosując **Podstawowe zasady przeprowadzania audytów bezpieczeństwa informacji**.

### Planowanie prac

Dokładny zakres prac dla poszczególnych etapów, biorąc pod uwagę specyfikę badanego OUK, określa Audytor Wiodący. Zadanie audytowe co do zasady składa się z dwóch etapów. Etapu 1 czyli zrozumienia kontekstu działania organizacji oraz analizy dokumentacji oraz Etapu 2 czyli przeprowadzeniu testów skuteczności funkcjonowania zabezpieczeń.

Biorąc pod uwagę specyfikę KSC koniczne jest przeprowadzanie w ramach zadania audytowego szeregu testów technicznych. Ich szczegółowy zakres oraz wielkość badanej próby powinny być zweryfikowany w trakcie Etapu I.

#### Etap I – Zrozumienie kontekstu działania organizacji oraz analiza dokumentacji

W trakcie Etapu I zespół audytowy koncentruje się na formalnej części wymagań oraz gromadzi wiedzę niezbędną do poprawnego przeprowadzenia testów skuteczności funkcjonowania zabezpieczeń podczas Etapu II.

Etap I powinien obejmować co najmniej następujące obszary:

1. zrozumienie zewnętrznego i wewnętrznego kontekstu funkcjonowania organizacji
2. weryfikacja przyjętego poziomu apetytu i tolerancji na ryzyko
3. weryfikacja przyjętej metodyki szacowania ryzykiem wystąpienia incydentu \(8.1 oraz 10.1\)
4. weryfikacja systematyczności procesu szacowania ryzykiem \(8.1\) i zgodności z przyjętą metodyką
5. weryfikacja procesu zarządzania ryzykiem bazując na zarejestrowanych ryzykach \(8.1 oraz 10.1\)
6. weryfikacja kompletności analizowanych ryzyk mogących prowadzić do wystąpienia incydentu \(8.1\)
7. weryfikacja relacji pomiędzy zidentyfikowanym ryzykiem a wdrożonymi mechanizmami kontrolnymi \(8.2\), w tym terminowości wdrożenia mechanizmów kontrolnych zidentyfikowanych w trakcie wcześniejszych audytów, kontroli oraz czynności procesu zarządzania ryzykiem
8. zidentyfikowanie i potwierdzenie poprawności udokumentowania mechanizmów kontrolnych zapewniających utrzymanie i bezpieczną eksploatację systemu informacyjnego \(8.2a oraz 10.1\)
9. zidentyfikowanie i potwierdzenie poprawności udokumentowania mechanizmów kontrolnych zapewniających bezpieczeństwo fizyczne i środowiskowe systemu informacyjnego \(8.2b oraz 10.1\)
10. zidentyfikowanie i potwierdzenie poprawności udokumentowania mechanizmów kontrolnych zapewniających kontrolę dostępu do systemu informacyjnego \(8.2b oraz 10.1\)
11. zidentyfikowanie i potwierdzenie poprawności udokumentowania mechanizmów kontrolnych zapewniających bezpieczeństwo i ciągłość dostaw usług od których zależy świadczenie usługi kluczowej \(8.2c oraz 10.1\)
12. zidentyfikowanie i potwierdzenie poprawności udokumentowania wdrożonych mechanizmów kontrolnych zapewniających ciągłe i niezakłócone świadczenie usługi kluczowej oraz zapewniających poufność, integralność, dostępność i autentyczność informacji \(8.2d oraz 10.1\)
13. potwierdzenie poprawności dokumentowania planów działania umożliwiających ciągłe i niezakłócone świadczenie usługi kluczowej oraz zapewniających poufność, integralność, dostępność i autentyczność informacji \(8.2d oraz 10.1\)
14. zidentyfikowanie i potwierdzenie poprawności udokumentowania mechanizmów kontrolnych zapewniających utrzymywanie ciągłe i niezakłócone świadczenie usługi kluczowej oraz zapewniających poufność, integralność, dostępność i autentyczność informacji \(8.2d oraz 10.1\)
15. zidentyfikowanie i potwierdzenie poprawności udokumentowania mechanizmów kontrolnych zapewniających monitorowanie systemu informacyjnego w trycie ciągłym \(8.2e oraz 10.1\)
16. zidentyfikowanie i potwierdzenie poprawności udokumentowania e mechanizmów kontrolnych zapewniających zbieranie informacji o zagrożeniach cyberbezpieczeństwa i podatnościach na incydenty systemu informacyjnego wykorzystywanego do świadczenia usługi kluczowej \(8.3 oraz 10.1\)
17. zidentyfikowanie i potwierdzenie poprawności udokumentowania mechanizmów kontrolnych zapewniających zarządzanie incydentami \(8.4 oraz 10.1\)
18. potwierdzenie skuteczności zgłaszania incydentów do odpowiednich organów \(8.4, 11 i 12\)
19. zidentyfikowanie i potwierdzenie poprawności udokumentowania mechanizmów kontrolnych zapewniających poufność, integralność, dostępność i autentyczność danych przetwarzanych w systemie informacyjnym \(8.5a oraz 10.1\)
20. zidentyfikowanie i potwierdzenie poprawności udokumentowania mechanizmów kontrolnych zapewniających aktualizację oprogramowania \(8.5b oraz 10.1\)
21. zidentyfikowanie i potwierdzenie poprawności udokumentowania mechanizmów kontrolnych zapewniających ochronę przed nieuprawnioną modyfikacją w systemie informacyjnym \(8.5c oraz 10.1\)
22. zidentyfikowanie i potwierdzenie poprawności udokumentowania mechanizmów kontrolnych zapewniających niezwłoczne podejmowanie działań po dostrzeżeniu podatności lub zagrożeń cyberbezpieczeństwa \(8.5d oraz 10.1\)
23. zidentyfikowanie i potwierdzenie poprawności udokumentowania dodatkowych mechanizmów kontrolnych zapobiegających oraz ograniczających wpływ incydentów na bezpieczeństwo systemu informacyjnego wykorzystywanego do świadczenia usługi kluczowej \(8.5 oraz 10.1\)
24. zidentyfikowanie i potwierdzenie poprawności udokumentowania mechanizmów kontrolnych zapewniających stosowanie środków łączności umożliwiających prawidłową i bezpieczną komunikację w ramach krajowego systemu cyberbezpieczeństwa systemu informacyjnego \(8.6 oraz 10.1\)
25. poprawność wyznaczenia i zgłoszenia osoby odpowiedzialnej za utrzymywanie kontaktów z podmiotami krajowego systemu cyberbezpieczeństwa \(9.1.1 oraz 9.1.3 oraz 9.2\)
26. poprawność zaprojektowania i udokumentowania procesu zapewnia użytkownikowi usługi kluczowej dostęp do wiedzy pozwalającej na zrozumienie zagrożeń cyberbezpieczeństwa i stosowanie skutecznych sposobów zabezpieczania się przed tymi zagrożeniami w zakresie związanym ze świadczoną usługą kluczową \(9.1.2 oraz 10.1\)
27. poprawność zaprojektowania i udokumentowania proces publikowania informacji pozwalającej na zrozumienie zagrożeń cyberbezpieczeństwa i stosowanie skutecznych sposobów zabezpieczania się na stronie internetowej \(9.1.2 oraz 10.1\)
28. poprawność proces aktualizacji dokumentacji dotyczącej cyberbezpieczeństwa \(10\)
29. poprawność ograniczania dostępu dokumentacji dotyczącej cyberbezpieczeństwa zgodnie z przyjętymi zasadami i przepisami prawa \(10.2\), w tym zapisów potwierdzających fakt wystąpienia zdarzeń
30. kompetencje, liczebność i charakter pracy wewnętrznych struktury odpowiedzialnych za cyberbezpieczeństwo lub umów zawartych z podmiotami świadczącymi usługi z zakresu cyberbezpieczeństwa pod kątem możliwości realizacji wymagań KSC oraz adekwatności do zidentyfikowanego ryzyka \(14.1 oraz 14.2.1 oraz 14.2.3\)
31. dostępność oraz poprawność zabezpieczenia pomieszczeń służących do świadczenia usług z zakresu reagowania na incydenty \(14.2.2 oraz 14.4\)

Na podstawie wniosków płynących z Etapu I audytor wiodący może zadecydować o zmianie wielkości próby badawczej dla poszczególnych testów Etapu II jak również modyfikacji zakresu tych testów, celem bardziej rzetelnego potwierdzenia skuteczności wdrożonych mechanizmów kontrolnych.

Etap I może być realizowany w sposób zdalny jeżeli istnieją odpowiednie warunki do bezpiecznego przekazania i analizowania otrzymanej dokumentacji.

**Analiza dowodów**

Zespół audytowy powinien dokonać analizy kompletności i skuteczności gromadzenia dowodów obejmujących co najmniej:

1. udokumentowane dowody na przyjęcie przez Najwyższe Kierownictwo apetytu i tolerancji na ryzyko
2. rejestr ryzyk \(8.1\)
3. udokumentowane dowody posiedzeń mających na celu szacowanie i zarządzanie ryzykiem \(8.1\)
4. rejestr incydentów \(8.1 oraz 8.4\)
5. udokumentowane dowody z procesu zarządzania zmianą systemu informatycznego \(8.2a\)
6. udokumentowane dowody z procesu zarządzania konfiguracją systemu informatycznego \(8.2a\)
7. udokumentowane dowody z testów bezpieczeństwa i ciągłości systemu informatycznego \(8.2a\)
8. udokumentowane dowody z testów bezpieczeństwa i ciągłości dostaw usług, od których zależy świadczenie usługi kluczowej \(8.2a\)
9. raporty z testów planów działania zapewniających ciągłe i niezakłócone świadczenie usługi kluczowej oraz zapewniających poufność, integralność, dostępność i autentyczność informacji \(8.2d\)
10. udokumentowane dowody systemów monitorujących system informatyczny wykorzystywany do świadczenia usługi kluczowej \(8.2e\)
11. udokumentowane dowody systemów gromadzących informacje o zagrożeniach cyberbezpieczeństwa \(8.3\)
12. udokumentowane dowody systemów gromadzących informacje o podatnościach na incydenty systemu informacyjnego \(8.3\)
13. udokumentowane dowody dokumentujące proces reagowania na incydenty zwykłe, poważne oraz krytyczne \(8.4 oraz 8.5a oraz 8.5c oraz 8.5d\)
14. udokumentowane dowody potwierdzające skuteczność procesu aktualizacji oprogramowania systemu informatycznego \(8.5b\)
15. zapisy potwierdzające skuteczność zapewniania użytkownikom dostępu do wiedzy \(9.1.2\)
16. opublikowane na stronie internetowej informacje pozwalającej na zrozumienie zagrożeń cyberbezpieczeństwa i stosowanie skutecznych sposobów zabezpieczania się \(9.1.2\)

#### Etap II – Testy skuteczności funkcjonowania mechanizmów kontrolnych

W trakcie Etapu II zespół audytowy koncentruje się na przeprowadzeniu testów skuteczności funkcjonowania mechanizmów kontrolnych zidentyfikowanych podczas Etapu I.

Zespół audytowy analizując zidentyfikowane mechanizmy kontrolne przede wszystkim bada ich poprawność zaprojektowania, czyli potwierdza, że są one w stanie realizować postawione cele. Następnie zespół audytowy bada czy mechanizm został poprawnie zaimplementowany.

Etap II powinien obejmować co najmniej następujące testy techniczne:

1. analiza podatności oprogramowania systemowego
2. analiza podatności aplikacji
3. analiza podatności sprzętu komputerowego
4. kolejne testy do dodania
5. 6. 7. 8. 9. potwierdzenie skuteczności gromadzenia udokumentowanych dowodów badanych w trakcie Etapu I
10. weryfikację kompletności identyfikacji i udokumentowania przez OUK mechanizmów kontrolnych zapewniających utrzymanie i bezpieczną eksploatację systemu informacyjnego \(8.2a\)

Etap II wymaga przeprowadzenia testów w badanych lokalizacjach, zgodnie z programem audytu.

Testy powinny obejmować :

1. Ochronę fizyczną,
2. Ochronę i prewencję zasobów ludzkich,
3. Ochronę aplikacji i systemów informacyjnych
4. Ochrona danych w zakresie bezpieczeństwa i RODO
5. 6. 7. 8. 
### Raportowanie

Raport z zadania audytowego powinien zawierać co najmniej

* podsumowanie dla kierownictwa
* listę obserwacji w zakresie niezgodności zawierającą klasyfikację zidentyfikowanego ryzyka oraz rekomendacje dla Kierownictwa OUK.

Klasyfikacja zidentyfikowanego ryzyka, w celu zapewniania porównywalności, powinna obejmować ryzyka:

Krytyczne - ….. użyć „incydentu krytycznego”

Wysokie - ….. użyć „incydentu krytycznego” i „poważnego”

Średnie - …… użyć „incydentu poważnego”

Niskie – …… użyć „incydentu zwykłego”

W przypadku raportów zawierających techniczne obserwacje rekomenduje się stosowanie skali CVSS.

Dobrą praktyką jest zapewnienie by wersja robocza raportu została merytorycznie zaopiniowana przez OUK w celu wyjaśnienia ewentualnych wątpliwości.

Raport z audytu jest zatwierdzany przez najwyższe kierownictwo OUK, które jest odpowiedzialne za zarządzanie ryzykiem zidentyfikowanych niezgodności.

