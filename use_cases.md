Słowem wstępu, wszystkie aplikacje, które będą przetwarzane przez wytwarzany w ramach projektu inżynierskiego produkt, mają być open source.

1. **[cwiczenia]** Aplikacja webowa, repozytorium, które pomaga nauczyć się budować systemy. Oprócz plików .py wykorzystuje również pliki .ipynb, a więc te od Jupitera. Korzysta również z plików .apkg. Plik APKG to niestandardowa talia fiszek stworzona do użytku w Anki, programie do nauki opartym na fiszkach.
    
    https://github.com/donnemartin/system-design-primer

- Nie ma Dockerfile
- Nie ma requirements

2. **[cwiczenia]** Algorytmy napisane w języku Python z różnych dziedzin: analiza arytmetyczna ( np. bisekcja ), filtry audio, operacje bitowe, algebra boola ( np. bramka and ), algorytmy szyfrowania, kompresja ( np. Huffman), konwersja jednostek, struktury danych

    https://github.com/TheAlgorithms/Python
- Posiada requirements
- Nie posiada Dockerfile

3. **[docker-compose][siec neruonowa][API Google]** Auto-GPT  - aplikacja open-source prezentująca możliwości modelu językowego GPT-4. Ten program, napędzany przez GPT-4, łączy ze sobą „myśli” LLM, aby samodzielnie osiągnąć dowolny cel. Wykorzystuje AI, chyba może być z cmd.
    
    https://github.com/Significant-Gravitas/Auto-GPT

- Posiada Dockerfile i docker_compose
- Posiada requirements plik
- Korzystać z brancha stable zamiast main
- Korzysta z API Google

4. **[pip][cmd]** Aplikacja cmd, która poprawia błędy w poprzednich poleceniach konsoli.

    https://github.com/nvbn/thefuck
- Posiada requirements
- Nie posiada Dockerfile
- Wymagane python3-dev, python3-pip, python3-setuptools, python 3.4+
- Można zainstalować przez pipa

5. **[Dockerfile][Web]** Aplikacja “Asystent Domu” pomagająca w zarządzaniu domem.

    https://github.com/home-assistant/core
- Posiada plik requirements
- Posiada własny Dockerfile
- Pisanie skryptów z wykorzystaniem yaml
- Jest opcja uruchomienia własnego OS
- Jest to serwer

6. **[pip]** System automatyzacji IT. Obsługuje zarządzanie konfiguracją, wdrażanie aplikacji, udostępnianie chmury, wykonywanie zadań ad-hoc, automatyzację sieci i orkiestrację wielu węzłów. Ansible sprawia, że złożone zmiany, takie jak aktualizacje kroczące bez przestojów, są łatwe dzięki systemom równoważenia obciążenia.

    https://github.com/ansible/ansible
- Można zainstalować poprzez pip
- Posiada plik requirements

7. **[CLI][Web]** Aplikacja webowa yt-dlp oparta na nieaktywnym youtube-dlc. Projekt dodaje nowe funkcje i poprawki przy jednoczesnym zachowaniu aktualności z oryginalnym projektem

    https://github.com/yt-dlp/yt-dlp
- Można zainstalować poprzez pip
- Posiada plik requirements
- Operuje jedynie w CLI
- Nie ma gotowego dockerfile

8. **[cwiczenia]** Projekt udostępniający ćwiczenia z zakresu DevOps. Zawiera głównie pytania z zakresu DevOps, jak i kilka ćwiczeń z pisania w Pythonie oraz Go. 

    https://github.com/bregman-arie/devops-exercises
- Nie posiada obrazu Dockera
- Nie ma pliku requirements


9. **[siec-neuronowa][GUI][GPU]** Aplikacja desktopowa będąca implementacją Transfer Learning from Speaker Verification to Multispeaker Text-to-Speech Synthesis (SV2TTS) z vocoderem, który działa w czasie rzeczywistym.
	
    https://github.com/CorentinJ/Real-Time-Voice-Cloning
- Aplikacja nie posiada Dockerfile
- Python 3.7 
- Potrzebuje ffmpeg i PyTorch.
- Wykorzystuje GPU do akceleracji.
- Posiada plik requirements.txt z zależnościami

10. **[CMD]** 
Sherlock: wyszukuje konta w mediach społecznościowych według nazwy użytkownika w sieciach społecznościowych

    https://github.com/sherlock-project/sherlock
- Bierze się z git clone 
- Na stronie githubowej jest instrukcja jak postawić aplikację w Dockerze
- Nie posiada gotowego image’a na Docker Hubie. Można go tylko samemu zbudować.
- Posiada plik requirements.txt, gdzie podane są wszystkie zależności do zainstalowania w formie Pythonowej (do instalacji pipem)
- Ma docker-compose w repozytorium
- Nie musi exposować żadnych portów

11. **[chat gpt][GUI]** 
GPT4free - Aplikacja będąca klonem GPT. 
    
    https://github.com/xtekky/gpt4free
- Ma możliwość używania GUI przez streamlit - framework do aplikacji webowych.
- Posiada gotowy build w docker hubie: gpt4free:latest. 
- Posiada plik requirements.txt, gdzie podane są wszystkie zależności do zainstalowania w formie Pythonowej (do instalacji pipem)
- Posiada docker-compose w repozytorium
- Porty: 8501:8501
- Potrzebuje ffmpeg
- Można ustawić proxy

12. Sentry - Platforma do śledzenia błędów i monitorowania wydajności, która pomaga zobaczyć błędy oraz szybciej rozwiązywać problemy.

    https://github.com/getsentry/sentry
- SDK do dużej ilości języków - w tym python
- Instalacja pip install
- To jest coś między stroną sentry.io a aplikacją, którą tworzymy
- Posiada coś takiego jak sentry relay, które jest warstwą pośrednią między aplikacją a stroną internetową - i to da się postawić na dockerze, wraz z configiem 
- Port 3000

13. **[chat gpt]** 
Open-Assistant - Aplikacja webowa której celem jest zapewnienie dostępu do modelu językowego opartego na czacie.
    
    https://github.com/LAION-AI/Open-Assistant
- Dostępne przez stronę internetową, ale dla developmentu można postawić lokalnie aplikację data collection.
- Dostępny docker-compose w repozytorium.

14. **[cmd] [web] [GUI]** 
mitmproxy - Projekt na repozytorium Github zawiera: interaktywny serwer proxy przechwytujący SSL/TLS z interfejsem konsoli dla HTTP/1, HTTP/2 i WebSockets, działającą w wierszu poleceń wersja powyższego serwera oraz internetowy interfejs do niego.

    https://github.com/mitmproxy/mitmproxy
- Posiada image na dockerhubie.
- Porty 8080, do webowej aplikacji również 8081

15. **[Let’s Encrypt] [CMD]** 
Certbot - przeznaczony do przełączania istniejącej witryny HTTP do pracy w HTTPS

    https://github.com/certbot/certbot
- Posiada image na dockerhubie
- Ma dużo opcji konfiguracji, np. Plugin standalone potrzebuje portów 80 i 443. 

16. **[CMD]** 
HTTPie - Klient HTTP uruchamiany z wiersza poleceń. Jest przeznaczony do testowania, debugowania i ogólnej interakcji z interfejsami API i serwerami HTTP. 

    https://github.com/httpie/httpie
- Python 3.7 albo wyżej
- Można zainstalować przez pip
- Nie posiada dockerfile ani docker-compose.

17. **[Jupyter] [Ćwiczenia]**
Interactive Coding Challenges - Zadania/wyzwania programistyczne w Jupiterze.
    
    https://github.com/donnemartin/interactive-coding-challenges
- Jupytera da się stawiać za pomocą docker run, są oficjalne obrazy do stawiania.

18. **[CMD] [SQL]** 
SQLMap - Narzędzie do testów penetracyjnych typu open source, które automatyzuje proces wykrywania i wykorzystywania luk wstrzykiwanych SQL oraz przejmowania serwerów bazodanowych. 

    https://github.com/sqlmapproject/sqlmap
- Jest wyposażony w silnik wykrywania, umożliwia pobieranie danych z bazy danych, dostęp do bazowego systemu plików itp.
- Python 2.6, 2.7 albo 3.x
- Można też zip/tar pobrać
- Można po prostu zbudować samemu obraz z aplikacji

19. **[sieci neuronowe] [GPU]** 
Fairseq - Zestaw narzędzi do modelowania sekwencji, który umożliwia trenowanie niestandardowych modeli do tłumaczenia, podsumowania, modelowania języka i innych zadań związanych z generowaniem tekstu.

    https://github.com/facebookresearch/fairseq
- Wymaga PyTorcha przynajmniej 1.10.0
- Potrzebne Nvidia gpu i NCCL
- Dla lepszego trenowania trzeba zainstalować również bibliotekę apex od Nvidii
- If you use Docker make sure to increase the shared memory size either with --ipc=host or --shm-size as command line options to nvidia-docker run.
- Nie posiada gotowego Dockerfile ani docker-compose

20. **[Może się przydać do naszego projektu i automatyzacji]**
Poetry - Pomaga deklarować, zarządzać i instalować zależności projektów Pythona, zapewniając wszędzie odpowiedni stos.

    https://github.com/python-poetry/poetry
- Instaluje się ze skryptu instalującego.
- Istnieje też możliwość instalacji przez pipx. 
- Wątki dotyczące dockeryzacji poetry:
    - https://stackoverflow.com/questions/53835198/integrating-python-poetry-with-docker 
    - https://medium.com/@harpalsahota/dockerizing-python-poetry-applications-1aa3acb76287 
    - https://python-poetry.org/docs/ 

21. **[web][REST API][SQL][wykresy]**
Wykorzystywany do eksploracji, wysyłania zapytań, wizualizacji i udostępniania danych z dowolnych źródeł (SQL).

    https://github.com/getredash/redash
- Dockerfile: tak
- requirements.txt: tak
- DockerCompose: tak
- potrzebne porty: tak 
- aplikacja wykorzystuje framework flask,  Jinja2 ( jest dostępna z poziomu przeglądarki)
- umożliwia tworzenie wizualizacji danych
- umożliwia udostępnianie wizualizacji i powiązanych z nim zapytań
- obsługuje ponad 35 źródeł danych SQL i NoSQL, można go również rozszerzyć, aby obsługiwać więcej

22. https://github.com/StevenBlack/hosts ???
- Dockerfile: tak
- requirements.txt: tak
- wersja Pythona:
- instalacja przez pip:
- potrzebne porty:
- zależności: 
- inne

23. **[cmd, wykresy, excel integration, GUI, GST API]**
Służy do badań inwestycyjnych
    
    https://github.com/OpenBB-finance/OpenBBTerminal
- requirements.txt: jest
- zapewnia automatyczną generację raportów
- ma też DiscordBota
- instalacja może być realizowana poprzez: installera 
- można instalować ze źródła (git) i aby to było możliwe trzeba wcześniej mieć zainstalowane następujące rzeczy: 
    - Miniconda (środowisko Pythona i menedżer pakietów), 
    - Git, 
    - Microsoft C++ Build Tools (Windows only), 
    - Rosetta2 (Apple Silicon only), 
    - LibOMP (Apple Silicon only), 
    - VcXsrv (Windows Subsystem for linux only), 
    - GTK toolchains (Linux only), 
    - do instalacji zależności i terminala odbywa się za pomocą Poetry
- instalacja za pomocą Dockera + żeby wyświetlić wykresy w kontenerze trzeba zainstalować VcXsrv
- oprócz terminala istnieje również OpenBB SDK - biblioteka Pythona, która zapewnia zestaw narzędzi do uzyskiwania dostępu do danych finansowych i przeprowadzania analiz finansowych. Tutaj instalacja się odbywa poprzez: PyPI albo ze źródła

24. **[web, cmd]** 
Bot do handlu kryptowalutami. Został zaprojektowany do obsługi wszystkich głównych giełd i może być kontrolowany przez Telegram lub webUI. Zawiera narzędzia do testowania wstecznego, kreślenia i zarządzania pieniędzmi, a także optymalizacji strategii poprzez uczenie maszynowe.

    https://github.com/freqtrade/freqtrade
- Dockerfile: tak
- requirements.txt: tak 
- DockerCompose: tak
- wersja Pythona: 3.8
- jest gotowy dokument jak uruchomić aplikację krok po kroku za pomocą Dockera (https://www.freqtrade.io/en/stable/docker_quickstart/)
- można pobrać zip/tar i samemu zainstalować 
- instalacja z conda
- potrzebne porty: tak

25. **[cmd][GPU]**
Szybki, bogaty w funkcje emulator terminala oparty na GPU.

    https://github.com/kovidgoyal/kitty
- prosta instalacja gotowych plików binarnych jednym poleceniem, jeśli wykorzystywany system to Linux lub MacOs
- można dokonać ręcznie instalacji lub ze źródła (git)
- można użyć menedżera pakietów, aby zainstalować pakiet kitty, ale trzeba mieć na względzie, że niektóre pakiety dystrybucyjne Linuksa są przestarzałe
- requirements.txt: brak, ale są napisane potrzebne rzeczy na odpowiedniej stronie
- brak Dockerfile

26. **[web][GUI][server]** 
Platforma handlowa GraphQL zapewniająca ultraszybkie, dynamiczne i spersonalizowane zakupy.

    https://github.com/saleor/saleor
- Dockerfile: tak
- requirements.txt: tak
- wersja Pythona: 3.8
- instalacja odbywa się poprzez sklonowanie repozytorium oraz zastosowanie Dockera
- możliwa też instalacja ręczna: Nodejs, Postgre SQL, GTK+
- można konfigurować Saleor za pomocą zmiennych środowiskowych

27. **[GUI][cmd][server]**
Menedżer e-booków. Może przeglądać, konwertować, edytować i katalogować e-booki we wszystkich głównych formatach e-booków. Może łączyć się z Internetem i pobierać metadane książek. Może pobierać gazety i konwertować je na e-książki w celu wygodnego czytania

    https://github.com/kovidgoyal/calibre
- Dockerfile: brak
- requirements.txt: brak
- wersja Pythona: 3.8
- instalacja poprzez stronę internetową ( w zakładce download na Windows, MacOs, Linux, Portable i też na aplikacje mobilne - Android oraz iOS)
- ma cmd dla wszystkich swoich funkcji - wykorzystywane w przypadku modyfikowania kodu
- jeśli chce się modyfikować kod to należy pobrać kod z gita
- pisze się tutaj wtyczki rozszerzające możliwości aplikacji, np. można pisać sterowniki: “For example, adding support for a new device to calibre typically involves writing less than a 100 lines of code in the form of a device driver plugin. ”

28. **[cmd]**
Szybszy sposób poruszania się po systemie plików. Działa poprzez utrzymywanie bazy danych katalogów, które są najczęściej używane z wiersza poleceń.

    https://github.com/wting/autojump
- Dockerfile: brak 
- requirements.txt: brak
- wersja Pythona: >=2.6 lub >= 3.3
- instalacja ręczna - pobranie z gita, przejście do odpowiedniego katalogu i wykonanie komendy ./install.py
- autojump jest również dostępny w niektórych dystrybucjach Linuksowych, np. Debian, Ubuntu, Linux Mint, RedHat, Fedora, CentOS, Slackware
- na MacOs instalacja za pomocą brew install

29. **[web]** 
Do zarządzania biznesem. Zbudowany na Frappe Framework, pełnym frameworku aplikacji internetowych zbudowanym z Pythonem i JavaScript.

    https://github.com/frappe/erpnext
- Dockerfile: brak 
- requirements.txt: brak

30. Wtyczka linii statusu dla vima, która zapewnia linie statusu i monity dla kilku innych aplikacji, w tym zsh, bash, fish, tmux, IPython, Awesome, i3 i Qtile
    
    https://github.com/powerline/powerline

31. Szanujący prywatność, możliwy do zhakowania silnik metasearch

    https://github.com/searx/searx

32. **[web]** Służy do modelowania i dokumentowania nowoczesnych sieci.

    https://github.com/netbox-community/netbox

33. Internetowy interfejs użytkownika, interfejs API REST i silnik zadań zbudowany na bazie Ansible. Jeden z projektów nadrzędnych dla Red Hat Ansible Automation Platform.

    https://github.com/ansible/awx

34. **[web]** Generacja stos backendu i frontendu za pomocą Pythona, w tym interaktywnej dokumentacji API.

    https://github.com/tiangolo/full-stack-fastapi-postgresql

35. **[web]** Serwer domowy Matrix o otwartym kodzie źródłowym.

    https://github.com/matrix-org/synapse

36. Umożliwia wykonywanie instrukcji podobnych do SQL bezpośrednio na tabelarycznych danych tekstowych, automatyczne buforowanie danych w celu przyspieszenia dodatkowych zapytań dotyczących tego samego pliku oraz wykonywanie instrukcji SQL bezpośrednio w wieloplikowych bazach danych sqlite3, bez konieczności ich scalania lub ładowania do pamięci

    https://github.com/harelba/q

37. Narzędzie do automatyzacji analizy open source (OSINT). Integruje się z niemal każdym dostępnym źródłem danych i wykorzystuje szereg metod analizy danych, ułatwiając nawigację po danych. Ma wbudowany serwer sieciowy zapewniający przejrzysty i intuicyjny interfejs internetowy, ale może być również używany całkowicie za pomocą wiersza poleceń. Jest napisany w Pythonie 3 i na licencji MIT.

    https://github.com/smicallef/spiderfoot

38. **[cmd]** Deduplikujący program do tworzenia kopii zapasowych. Opcjonalnie obsługuje kompresję i uwierzytelnione szyfrowanie.

    https://github.com/borgbackup/borg

39. **[GUI]** Wieloplatformowy graficzny interfejs użytkownika popularnego programu do pobierania multimediów youtube-dl napisany w wxPython.

    https://github.com/MrS0m30n3/youtube-dl-gui


### Generowanie Dockerfile z użyciem modelu GPT
Korzystając z chatu GPT można wygenerować prosty plik Dockerfile oraz docker-compose.yaml, jednak wymagany jest do tego dokładny opis konteneryzowanej aplikacji (zależności, komendy, wersje, udostępniane porty, czy potrzebuje GPU i inne specyfikacje) NIe mniej jednak korzystając z modelu 3.5 jest masa problemów, i w praktyce nie nadaje się on do łatwego stowrzenia skomplikowanego pliku. Jest to bardziej metodyka prób i błędów.
