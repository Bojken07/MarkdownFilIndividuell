#Beskrivning vad jag har bidragit med under grupparbetet: Jag har bidragit med att hjälpa och skriva kod som 
behövdes för att blir klart med projektet. Jag har varit närvaro på alla möte och samlingar som vi har haft 
med teamet. 

#Vilken kod har jag bidragit med: Jag har bidragit med några Mappningar och Controllers i GetControllers klassen
samt i HTML.Pages. T.ex som (home sidan, search, logut-success, anonymize Email, Email.DTO klass, MaskingUtils class).

#Beskriv utförligt vad just min kod gör, ge kodexempel med kodblock och förklara vad
koden gör:
            

              ```java
              
                public class EmailDTO {

                private String email;

                public String getEmail() {
                return email;
               }

                public void setEmail(String email) {
                this.email = email;
                }
              }

                       ```


Koden definierar en klass som vi har kallad EmailDTO.
Förklaring av koden: Public betyder att är synlig och vi kan andendar från alla andra klasser.
EmailDTO: EmailDTO classen deklarerar en klass med namnet EmailDTO. Den klassen vi använder 
för att representera dataöverföring (Data Transfer Object) för e-postadresser.
Private: Private anger att variabeln email endast är tillgänglig inom denna klass. 
Ingen annan klass kan direkt komma till denna variabel.
String email: Detta deklarerar en instansvariabel av typen String med namnet email. Denna variabel används
för att lagra en e-postadress.
public: Åtkomstmodifieraren public anger att metoden är tillgänglig för alla andra klasser.
String getEmail(): Den deklarerar en metod som returnera en string.
return email;: Metoden returnerar värdet av instansvariabeln email. Det gör det möjligt för dom andra klasser 
att få värdet på email utan att komma direkt till den privata variabeln.
void setEmail(String email): Detta deklarerar en metod som tar en parameter av typen String och returnerar inget 
(void). this.email = email;: Denna rad tilldelar värdet på parameter email till instansvariabeln email. this
refererar till den aktuella instansen av klassen, vilket hjälper till att skilja mellan instansvariabeln och
metodparametern med samma namn.


#Svar på fråga 1: 

                   ```java

              @GetMapping("/register/user")
    public String registerUser(Model model) {
        model.addAttribute("user", new UserDTO());
        logger.debug("Accessing the register user page.");
        return "registerUser";
    }
                           ```

#Svar på fråga 2: Public på en metod betyder att metoden är deklarerad som public och kan nås från alla
                  andra klasser och objekt, oavsett var befinner sig i applikationen. Det är tillgäglig globalt.
                  Privat på en metod betyder att metoden är deklarerad som privat och kan endast nås från inom
                  den klass där den är deklarerad. Som private den är osynlig och otillgäglig för andra klasser.

 Exempel Public:  

                      ```java
                      public class MyClass {
                      public void myPublicMethod() {
                        // Kod som kan anropas från vilken annan klass som helst
                       }
                      }        
                                   ```         
                     
 Exempel Private: 
 
                     ```java
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

Exempel void: 

                  ```java
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

#Svar på fråga 6: Dom  kallas argument eller parametrar. En parameter är en variabel i metoddefinitionen som fungerar
                  som en platsmottagare för värdena som skickas till metoden. Ett argument är värdet eller 
                  referensen som skickas till metoden när den anropas.
                 

Exempel med parametrar och argument: 

                  ```java
                  public class MyClass {

                  // Metod med två parametrar
                   public void addNumbers(int a, int b) {
                   int sum = a + b;
                   System.out.println("Sum: " + sum);
                   }

                   public static void main(String[] args) {
                   MyClass obj = new MyClass();

                   // Anrop av metod med två argument
                   obj.addNumbers(5, 7);  // 5 och 7 är argument som skickas till metoden
                        }
                    }              
                               ```

#Svar på fråga 7: Jag tror att det ska blir rätt och det ska returneras resultatet som vi behöver om det plir int
                  istället för void som det skrivs i koden.
Exempel metod i koden: 

                      ```java
                      public int add(int a, int b){
                      int sum = a + b;
                      return sum;
                      }
                              ```

#Svar på fråga 8: Exempel när man anropar denna metod från en annan metod:

                       ```java
                 public class Main {

                 // Annan metod som anropa add-metoden.
                public void performAddition() {
                int num1 = 4;
                int num2 = 9;

                // Anropa add-metoden och spara resultatet i en variabel.
                MyClass obj = new MyClass();
                int result = obj.add(num1, num2);

                // Skriv ut resultatet
                System.out.println("Resultatet av additionen är: " + result);
                }

                 public static void main(String[] args) {
                Main mainObj = new Main();
                mainObj.performAddition();
                   }
                }
                            ```

#Svar på fråga 9: Din class med tom konstruktor:

                  ```java
                  public class HakansClass {
                  // Tom konstruktor
                  public HakansClass() {
                   // Tom kropp utan argument
                     }
                  }
                           ```

#Svar på fråga 10: Primitiva typer lagras direkt i minnen, dom representerar enkla värden och dom
                   är inte objekt. 
Exempel med primitiv typ:

                     ```java
                      // Primitiv typ med ett värde
                     int number = 4;
                            ```
Exempel med typ objekt: Objekt  representerar komplexa datastrukturer och är instanser av klasser.
                        De lagras i minnet via referenser.

                    ```java
               // Skapande av ett objekt (en instans av en klass)
               MyClass obj = new MyClass();
                            ```

#Svar på fråga 11: Metoden börjar med ett verb som beskriver vad metoden utför eller gör, exempel 'additionSum'.
                   Om du använda en verbform som början av metodnamnet kan du tydligt ange vad metoden gör och
                   det blir lättare för andra utvecklare att förstå dess syfte.

Två exemplar med kodblock: 
 
                    ```java
                    public class MyClass {

                   // Metod för att beräkna summan av två tal
                   public int calculateSum(int a, int b) {
                   return a + b;
                   }

                   // Metod för att skriva ut ett meddelande till konsolen
                   public void printMessage(String message) {
                   System.out.println(message);
                   }
                             ```


#Svar på fråga 12: @Override används i Java för att markera en metod som överskriver en metod i en överordnad klass 
                   eller implementerar en metod från ett interface.

#Svar på fråga 13: Vi kan kalla på den metoden i subklassen i MyCustomAuthenticationProvider?: Ja, vi kan kalla den metoden som är 
deklarerad i superklassen, för att göra detta vi måste använda nyckelordet (super) för att referera till superklassens 
medlemmar.

Kodexempel:

                        ```java

              public class MyCustomAuthenticationProver extends DaoAuthenticationProvider{
                 public MyCustomAuthenticationProver(){
                    }
                   public void someMethod() {
        
                Authentication auth = ; // Här vi kan skapa en objekt
                Authentication result = super.authenticate(auth);
                  }
               }


#Svar på fråga 14: PasswordEncoder har för uppgift för att kryptera lösenord och verifiera lösenordmatchningar. Det är en 
viktig komponent i Spring Security som används för att kryptera lösenord och verifiera lösenordmatchningar.
Användning av PasswordEncoder i @Bean: I Spring-applikationer konfigureras PasswordEncoder vanligtvis som en @Bean.
Detta görs i konfigurationsklasser eller konfigurationsfiler.


#Svar på fråga 15:  
 
                        ```xml

            <?xml version="1.0" encoding="UTF-8"?>
           <configuration>

                <!-- Vanlig fil-appender -->
           <appender name="FILE" class="ch.qos.logback.core.FileAppender">
           <file>myapp.log</file> <!-- Namnet på den vanliga loggfilen -->
           <append>true</append>
        <encoder>
            <pattern>%d{yyyy-MM-dd HH:mm:ss.SSS} [%thread] %-5level %logger{36} - %msg%n</pattern>
        </encoder>
    </appender>

    <!-- ROLLING file-appender -->
    <appender name="ROLLING" class="ch.qos.logback.core.rolling.RollingFileAppender">
        <file>myapp.%d{yyyy-MM-dd}.log</file> <!-- Mönster för filnamn som inkluderar datum -->
        <encoder>
            <pattern>%d{yyyy-MM-dd HH:mm:ss.SSS} [%thread] %-5level %logger{36} - %msg%n</pattern>
        </encoder>
        
        <rollingPolicy class="ch.qos.logback.core.rolling.TimeBasedRollingPolicy">
            <!-- Loggfilens namnformat -->
            <fileNamePattern>myapp.%d{yyyy-MM-dd}.log</fileNamePattern>
            <!-- Antal dagar att behålla loggfilerna -->
            <maxHistory>30</maxHistory>
        </rollingPolicy>
    </appender>

    <!-- Logger för paketet se.sprinto.hakan.securityapp som använder ROLLING file-appender -->
    <logger name="se.sprinto.hakan.securityapp" level="DEBUG">
        <appender-ref ref="ROLLING"/>
    </logger>

    <!-- Root-logger som använder den vanliga file-appender -->
    <root level="INFO">
        <appender-ref ref="FILE"/>
    </root>

     </configuration>

                      ```



#Svar på fråga 16: 200 OK: Begäran har lyckats och resursen returneras.
                   401 Unauthorized: Begäran kräver autentisering. Användaren är inte autentiserad.
                   403 Forbidden: Begäran är förbjuden. Användaren är autentiserad men har inte tillräckliga rättigheter.
                   404 Not Found: Den begärda resursen kunde inte hittas på servern.