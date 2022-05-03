# spotted-bot-dc
$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$

By twój bot działał w polskiej wersji skopiuj pliki z tego katalogu do katalogu data

$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$

CREATED BY: Abstergo using Discord Bot Maker

$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$
UWAGA: PRZECZYTAJ TO PRZED URUCHOMIENIEM BOTA
#################################################################################################
WSTĘP

Ten bot tworzy infrastrukturę spotted na twoim serwerze, zawiera ona
2 kanały i jedną rolę:

1. kanał Spotted	- po użyciu komendy /spotted bot wysyła tutaj anonimową wiadomość użytkownika

2. kanał Logs		- tylko administrator go widzi
			- wysyłane są tutaj logi z kanału spotted razem z nadawcą wiadomości i załącznikiem
			- jedyny sposób by karać troli
3. rola Troll		- stworzona by napiętnować troli, zabrania im używania komendy spotted oraz czytania kanału
#################################################################################################
Inne komendy

/rc - odtwarza infrastrukturę spotted (na wypadek zdrady jednego z adminów)

/cl - dzięki niej mozesz masowo kasować wiadomości z kanałów

/nsfw - komenda tworząca dodatek nsfw
####################################################################################################
/nsfw 

Tworzy jednen kanał i jedna rolę:
1. nsfw channel - dokładnie taki jak spotted ale przeznaczony dla materiłów 18+
2. nsfw spotter role - pozwala użytkownikom używać tego dodatku (sam zdecyduj komu ją dać)
###################################################################################################
Konfiguracja bota:

Muszisz zrobić to sam,
1. wejdź na https://discord.com/developers/applications
2. stwórz aplikacje bota, nazwij ją jak chcesz
3. znajdź 'app id' i 'bot token'
4. wejdź w  'lokalizacja bota'/data/settings.json
5. wprowadź dane z punktu 3. we wskazane pola
6. zapisz plik
####################################################################################################
Start twojego bota

1 metoda - na własnym komputerze (twój komputer będzi musiał cały czas działac by bot był online)(DARMOWA)

- zainstaluj node.js i uruchom go
- w konsoli wpisz: node 'lokalizacja bota'/bot.js
- gotowe
- możesz dodać bota do servera

2 metoda - na heroku (DARMOWA)
- stwórz Procfile i umieść go w lokalizacji bota
- w procfile wpisz 'worker: node bot.js'
- prześlij pliki na heroku
- zmień dyno formation na worker 
- możesz dodać bota na server

By dodać pota na server wklej ten link w przeglądarkę: https://discord.com/api/oauth2/authorize?client_id=YOUR BOT APP ID&permissions=8&scope=bot%20applications.commands
################################################################################################################

Możesz wprowadzać zmiany w moim bocie, jednak jako że zostal on stworzony przy użyciu aplikacji Discord Bot Maker, może to być ciężkie nie używając jej,
Każdy prawdziwy programista powinin raczej napisac swojego bota od zera zamiast go przerabiać

####################################################################################################################
