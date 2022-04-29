# spotted-bot-dc
##############################################################################################################################################################


By twój bot działał w wersji po polsku zwtczajnie podmień pliki commands.json i events.json w folderze data na te załączone tutaj


################################################################################################################################################################# 
$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$

CREATED BY: Abstergo using Discord Bot Maker

$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$
WAŻNE: PRZECZYTAJ TO ZANIM URUCHOMISZ BOTA
#####################################################################################################################################################################
WSTĘP

Ten bot tworzy infrastrukturę spotted na twoim serverze dc
gdy dołączy do niego stworzy 3 kanały i 1 rolę

1. kanał post		- można tu wysyłać swoje wiadomości, są one od razu ususwane
			- by załączyć obraz należy wpisać 'img' w treść wiadomości, jeżeli z kolei nie załączasz pliku proszę użyć innego wyrażenia
			- nie można załączać żadnych innych plików
			- bot będzie wysyłał wiadomość: 'Wyciszyłeś ten kanał?' co każde 15 minut, i od razu je usuwał, użytkownik który nie wyciszył kanału, 
			  będzie więc otrzymywał spam, on i tylko on

2. kanał spotted	- bot wysyla tutaj anonimowe wiadomości użytkowników

3. kanał logs		- tylko administrator widzi ten kanał
			- wysyłane są tu te same wiadomosci co na kanał spotted ale zawierają one authora
			- tylko ten kanał zapewnia możliwosć karania trolli

4. rola ruskiego trolla	- jako że domyślnie każdy może używać spotted ta rola powstała by oznaczyć tych którym zostało to prawo odebrane
###################################################################################################################################################################
Inne komendy

!rc - odtwarza kanały post, logs i spotted (na wypadek zdrady jednego z adminów)(odtworzone kanały nie zawierają wcześniej wysłanych wiadomości)

!cl x y - zwykła wiadomość do czyszcenia - może się zdarzyć że wiadomość przypominająca nie zostanie usunięta,a lbo twój osting przestanie działać wieć 
	  ta komenda pozwala usuwać wiadomosci masowo, x oznacza liczbę wiadomosci do usunięcia na kanale post, y jest dla kanału nsfw (czytaj dalej)

!nsfw - dodatek - tworzy drugą infrastrukturę spotted tyle że dla zawartości nsfw
#####################################################################################################################################################################
dodatek !nsfw

Tworzy dwa kanały i jedna rolę
1. kanał nsfw		 - taki jak post ale dla nsfw (ukryty dla każdego bez roli)
2. kanał nsfw spotted	 - taki jak spotted ale dla nsfw (ukryty dla każdego bez roli)
3. rola nsfw spotter 	 - pozwala ludziom zobaczyć kanały nsfw insfw spotted
#######################################################################################################################################################################
Konfiguracja bota:

Muszisz zrobić to sam,
1. wejdź na https://discord.com/developers/applications
2. stwórz aplikacje bota, nazwij ją jak chcesz
3. znajdź 'app id' i 'bot token'
4. wejdź w  'lokalizacja bota'/data/settings.json
5. wprowadź dane z punktu 3. we wskazane pola
6. zapisz plik
##################################################################################################################################################################
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

PAMIĘTAJ BY WPIERW URUCHOMIĆ BOTA A POTEM DOPIERO DODAĆ GO DO SERVERA BO INACZEJ PODSTAWOWE KANAŁY NIE ZOSTANĄ STWORZONE

By dodać pota na server wklej ten link w przeglądarkę: https://discord.com/api/oauth2/authorize?client_id='your_app_id'6&permissions=8&scope=bot%20applications.commands
###################################################################################################################################################################

Możesz wprowadzać zmiany w moim bocie, jednak jako że zostal on stworzony przy użyciu aplikacji Discord Bot Maker, może to być ciężkie nie używając jej,
Każdy prawdziwy programista powinin raczej napisac swojego bota od zera zamiast go przerabiać

######################################################################################################################################################################
