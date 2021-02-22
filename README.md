Opis użytych adnotacji:

@GetMapping - adnotacja ta jest odpowiedzialna za mapowanie żądanie HTTP GET,
                po end-poincie /greeting do metody greeting().

@RequestParam - wiąże wartość nazwy parametru ciągu zapytania z parametrem name metody greeting(). 
                Jeśli w żądaniu nie ma parametru name, używana jest wartość defaultValue of World.

@RestController, która oznacza klasę jako kontroler, gdzie każda metoda zwraca obiekt domeny zamiast widoku. 
                Jest skrótem który uwzględnienia zarówno @Controller, jak i @ResponseBody.

@SpringBootApplication to wygodna adnotacja, która dodaje wszystkie poniższe elementy:

@Configuration: taguje klasę jako źródło definicji komponentów bean dla kontekstu aplikacji.

@EnableAutoConfiguration: nakazuje programowi Spring Boot rozpoczęcie dodawania komponentów bean na podstawie ustawień ścieżki klas, 
innych komponentów bean i różnych ustawień właściwości. Na przykład, jeśli spring-webmvc znajduje się na ścieżce klasy, 
ta adnotacja oznacza aplikację jako aplikację internetową i aktywuje kluczowe zachowania, 
takie jak konfigurowanie DispatcherServlet.

@ComponentScan: nakazuje Springowi wyszukanie innych komponentów, 
konfiguracji i usług w pakiecie com / example, pozwalając jej znaleźć kontrolery.