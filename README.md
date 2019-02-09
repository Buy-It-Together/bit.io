# Buy It Together

<iframe width="560" height="315" src="https://www.youtube.com/embed/q-Rxgnw7PV4" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

Buy It Together to aplikacja do agregacji ofert użytkowników na wyznaczonym przez nich samych terenie. Przykładowo jeżeli jesteśmy zainteresowani kupnem danego produku dodajemy nową ofertę w aplikacji mobilnej. Aplikacja pozwala na znalezienie osób zainteresowanych danym produktem na wyznaczonym terenie. Dzięki czemu możemy kupić przedmioty wspólnie. Zaszczędzamy na kosztach przesyłki, a w niektórych przypadkach można uzyskać promocję od sprzedającego.  

## Bit client
[Download Android BIT client version 1.0.0](https://github.com/Buy-It-Together/Android-BIT-Client/releases/download/v1.0.0/BITv1.0.0.apk)

## Wymagania biznesowe
Aplikacja agreguje konsumentów chcących kupić drogą internetową ten sam produkt. Agregacja odbywa się na terenie wyznaczonym przez odbiorców. Po zsumowaniu ofert użytkowników system wysyła zaproszenie do czatu. Użytkownik ma możliwość podglądu sugerowanej lokalizacji spotkania. Po akceptacji zaproszenia do czatu użytkownicy mogą się komunikować w czasie rzeczywistym. Interfejs aplikacji jest w języku angielskim.

## Dziedzinowy słownik pojęć
-	Użytkownik – osoba korzystająca z aplikacji
-	Link – adres do strony internetowej z ofertą.
-	Oferta – zdefiniowana przez użytkownika chęć nabycia danego przedmiotu wskazanego pod podanym wcześniej linkiem.
-	Czat – definiuje zbiór użytkowników, którzy chcą nabyć dany produkt. 
-	Zaproszenie do czatu – informacja o możliwości dołączenia do czatu. 

## Wymagania funkcjonalne
- Użytkownik jest uwierzytelniany na podstawie adresu email oraz hasła. Podczas procesu rejestracji użytkownik musi kliknąć w link aktywacyjny wysłany na podany wcześniej adres email.
-	Hasło użytkownika jest zapisywane w bazie danych w sposób niejawny
-	Każdy użytkownik może dodać ofertę. Wprowadzone dane muszą podlegać walidacji. Adres docelowy ma być zamieniany z formy czytelnej dla użytkownika na współrzędne geograficzne. Podczas definiowania oferty należy wypełnić pola:
  - Link do przedmiotu.
  - Adres docelowy. 
  -	Dystans, który użytkownik może pokonać w celu odebrania przedmiotu.
  - Liczbę produktów, których użytkownik chcę nabyć.
  - Liczbę produktów potrzebnych do uzyskania promocji.
  -	Datę ważności oferty.
-	Każdy użytkownik może przeglądać swoje oferty. 
-	Po zagregowaniu ofert użytkownik dostaje zaproszenie do czatu. Użytkownik może zobaczyć proponowaną lokalizację przed zaakceptowaniem zaproszenia.
-	Po akceptacji zaproszenia użytkownik ma możliwość komunikacji się w czasie rzeczywistym z pozostałymi użytkownikami czatu. 
## Wymagania niefunkcjonalne
-	Użytkownik powinien mieć możliwość korzystania z aplikacji na platformach mobilnych z systemem Android. 
-	Użytkowanie systemu powinno być intuicyjne i wygodne dla użytkownika.
-	Aplikacja nie powinna zbędnie zużywać baterii.
-	System powinien być dostępny o każdej porze dnia.
-	Aplikacja powinna korzystać z darmowych rozwiązań.
-	System powinien pozwolić na zaimplementowanie klientów na inne platformy niż Android bez ingerowania w kod źródłowy serwera.
## Reguły biznesowe
- Jeżeli czas zalogowanego użytkownika do aplikacji przekroczy domyślny zdefiniowany czas sesji po stronie serwera użytkownik musi powtórzyć operację logowania się.
- Brak limitu na dodawanie ofert przez użytkownika. 
- Brak limitu wysyłanych przez system zaproszeń dotyczących ofert.
- Tylko jedno zaproszenie odnoszące się do oferty może być zaakceptowane. 
- Osoba niezalogowana do systemu nie ma możliwości korzystania z niego. Wyjątkiem są funkcjonalności rejestrowania oraz logowania. 

## Specification of requirements
The application aggregates consumers who want to buy the same product online. Aggregation takes place in the area designated by the recipients. After summing up user offers, the system sends a chat invitation. The user can preview the suggested location of the meeting. After acceptance of the chat invitation, users can communicate in real time.

## A domain dictionary of concepts
- User - a person using the application
- Link - the address of the website with the offer.
- Offer - user defined desire to purchase a given item indicated under the link provided above.
- Chat - defines a set of users who want to purchase a given product.
- Chat invitation - information about the possibility of joining a chat.

## Functional requirements
- The user is authenticated based on the email address and password. During the registration process, the user must click on the activation link sent to the previously provided email address.
- The user's password is stored in the database in an undisclosed way.
- Each user can add an offer. The data entered must be validated. The destination address is to be converted from a user-readable form to geographical coordinates. When defining an offer, fill in the fields:
  - Link to the subject.
  - Destination address.
  - Distance that the user can overcome in order to pick up the item.
  - The number of products that you want to buy.
  - The number of products needed to get the promotion.
  - The offer expiration date.
- Each user can view their offers.
- After aggregating the offers, the user gets an invitation to chat. The user can view the proposed location before accepting the invitation.
- After accepting the invitation, the user can communicate in real time with other chat users.

## Non-functional requirements
- The user should be able to use the application on mobile platforms with Android.
- Use of the system should be intuitive and convenient for the user.
- The application should not use batteries unnecessarily.
- The system should be available at any time of the day.
- The application should use free solutions.
- The system should allow clients to be implemented on platforms other than Android without interfering with the server's source code.

## Business rules
- If the time of the logged-in user to the application exceeds the default defined session time on the server side, the user must repeat the login operation.
- No limit on the user adding offers.
- No limit of invitation invitations sent by the system.
- Only one invitation relating to the offer can be accepted.
- A person who is not logged into the system is not able to use it. The exception is the logging and logging functionality. 
