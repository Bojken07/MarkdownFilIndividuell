#Beskrivning vad jag har bidragit med under grupparbetet:



#Vilken kod har jag bidragit med:



#Beskriv utförligt vad just min kod gör, ge kodexempel med kodblock och förklara vad
koden gör:






#Svar på fråga 1:




#Svar på fråga 2: Public på en metod betyder att metoden är deklarerad som public och kan nås från alla
                  andra klasser och objekt, oavsett var befinner sig i applikationen. Det är tillgäglig globalt.
                  Privat på en metod betyder att metoden är deklarerad som privat och kan endast nås från inom
                  den klass där den är deklarerad. Som private den är osynlig och otillgäglig för andra klasser.

 Exempel Public:      ```java
                      public class MyClass {
                      public void myPublicMethod() {
                        // Kod som kan anropas från vilken annan klass som helst
                       }
                      }        
                                   ```         
                     
 Exempel Private:    ```java
                     public class MyClass {
                     private void myPrivateMethod() {
                        // Kod som endast kan anropas inom denna klass
                      }
                                   ```

#Svar på fråga 3: Om en metodsignatur innehåller void betyder att metoden inte returnerar något värde.
                  Void används när metoden utför en uppgift men inte behöver skicka tillbaka något resultat
                  till den som anropar metoden. Om en metodsignatur innehåller en typ (som en primitiv typ:int,
                  float, boolean, etc.) eller en klass(som String, List,etc.) betyder att metoden returnerar ett 
                  värde av den typen eller klassen.

Exempel void:     ```java
                  public void printMessage() {
                  System.out.println("Hej, världen!");
                  }
                                  ```

                  MyClass obj = new MyClass();
                  obj.printMessage(); // Skriver ut "Hej, världen!" men returnerar inget värde
                                  ```

#Svar på fråga 4: Det finns 4 namnkonvention metoder i Java.
                  Dom är: "Camel Case", Metodnamn bör använda camel case, vilket innebär att det första ordet börjar
                          med en liten bokstav och varje efterföljande ord börjar med en stor bokstav utan mellanslag.
                          Exempel: 'getUserName'.
                          "Små Bokstäver",  Använd små bokstäver för det första ordet och stora bokstäver för början
                          av varje efterföljande ord. Exempel: 'calculateArea'.
                          "Beskrivande Namn", Namnet på metoden bör vara beskrivande och tydligt förklara vad metoden 
                          gör. Undvik att använda förkortningar och kryptiska namn. Exempel: 'processOrder' 
                          "Verb som Första Ord".  Metodnamn bör börja med ett verb som beskriver vad metoden gör.
                          Detta gör koden mer beskrivande och lättare att förstå. Exempel: 'calculateTotal'.
                  

#Svar på fråga 5: Om det inte står något mellan parenteserna () efter metodens namn i Java, innebär det att metoden inte
                  tar några argument.

                 ```java
                 public class MyClass {

                 // En metod som inte tar några argument och inte returnerar något
                 public void printHello() {
                  System.out.println("Hello, World!");
                 }                                     
                                 ```




#Svar på fråga 6:



#Svar på fråga 7:



#Svar på fråga 8:



#Svar på fråga 9:



#Svar på fråga 10:



#Svar på fråga 11:
