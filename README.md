# Job

@Override – używana do oznaczania implementacji metod z interfejsów

@Valid – użyta w kontrolerze przy atrybucie metody powoduje, że obiekt ten jest traktowany jako formularz i uruchamiana jest jego walidacja (np. na podstawie poniższych adnotacji). Kolejny argument metody po tym musi być typu BindingResult – tam Spring umieści informacje o problemach

@NotNull – pole musi mieć wartość(nie może być nullem)

@NotBlank – pole nie może być czyste (np. wypełnione tylk białymi znakami)

@NotEmpty – pole nie może być puste

@Email – pole zawiera poprawny (od strony składni, niekoniecznie istniejący!) adres email

@RequestMapping – mapuje adres URL i/lub metodę HTTP na metodę kontrolera

@ResponseBody – Spring stara się przekształcić zwrócone wartości w odpowiedź http (np. konwertując obiekt na format JSON lub XML)

@RequestBody, Spring  stara się przekształcić treść przychodzącego żądania w obiekt, np. kiedy chcemy otrzymać dane JSON i automatycznie je zamienić na obiekt.

@RequestParam – pozwala pobrać wartość parametru przekazywanego w adresie url np. “?userId=5”, do zmiennej

@PathVariable – obsługuje zmienną przekazaną w postaci fragmentu adresu url np. user/5 (user/{userId})

@Required – sprawdza, czy dane pole zostało ustawione (czy Spring wstrzyknął mu wartość) podczas uruchamiania

@Transactional – Pozwala zgrupować wiele czynności w ramach jednej transakcji bazy danych. Dzięki temu w przypadku niepowodzenia jednej z nich, pozostałe zostaną wycofane.

@Entity – Adnotacja, która mówi o tym, że ta klasa jest zarządzana przez JPA i odpowiada tabeli w bazie danych

@Table – Dzięki tej adnotacji możemy określić dodatkowe parametry związane z tabelą bazy danych, którą ta klasa reprezentuje. Możemy określić np. nazwę.

@Column – Analogicznie do @Table, ale pozwala nam określać atrybuty kolumn w tabeli w bazie danych, np. ich typ, długość, nazwę.
