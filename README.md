# crack-bucharest-interviews
Intrebari si probleme pe care le-am primit pana acum la interviuri. (Java Developer)

![](https://api.visitorbadge.io/api/VisitorHit?user=nicugnm&repo=crack-bucharest-interviews&countColor=%237B1E7A)
### Java Vanilla / Generale

1. Care este diferenta dintre o clasa abstracta si o interfata?
2. O clasa abstracta se poate instantia? Dar o interfata?
3. Un obiect poate avea mai multe clase? Dar o clasa poate avea mai multe obiecte? Descrie care este diferenta dintre o clasa si un obiect.
4. Cum functioneaza coliziunile intr-un HashMap in Java? Cum sunt tratate in spate? Key si value ce tip de date pot primi?
5. Ai folosit generice? Cand si cum? Cand folosim Generics in Java, cu ce keyword ne putem referi ca un obiect T este un subtip al obiectului? Dar un supertip? (Extends si super keywords din Generics)
6. Este var un keyword in Java?
7. Care este diferenta dintre Thread.run si Thread.start? Se creeaza un thread nou sau nu?
8. Ce este un deadlock? Cum putem obtine un deadlock in Java? (Producer & Consumer problem)
9. Ce este thread starvation si livelock? Cum putem obtine un thread starvation in Java si un livelock?
10. Ce este un thread starvation in Java?
11. Cum putem seta mai multe 'pools' unui thread in Java ? (--> Executor Service)
12. Cum putem face un thread in Java?
13. Diferenta dintre Thread.fork() si Thread.join() in Java?
14. Cate tipuri de exceptii sunt in Java?
15. Care este diferenta dintre programare concurenta si programare reactiva?
16. De ce se cheama polimorfism static/dinamic?
17. Ce structura de date foloseste cautare in O(log n)?
18. Cum putem sorta o lista in Java?
19. Doua obiecte egale au acelasi hashcode?
20. Diferenta dintre SpringBuilder si StringBuffer
21. Diferenta dintre HashMap si TreeMap si Hashtable, ce este un hashmap? + complexitati
22. Diferenta dintre HashSet si TreeSet si ce este un hashset? + complexitati
23. Diferenta dintre ArrayList si LinkedList, descriere + complexitati
24. Ce se intampla daca ai intr-un hashmap toate elementele cu un hashcode null, ce se intampla la inserare si care e complexitatea? Cum functioneaza in spate hashmap-ul, load factor si capacity?
25. Cum putem face o clasa imutabila?
26. Cum se face o clasa singleton?
27. Ce design pattern putem avea pentru a crea o singura instanta daca apelam clasa cu mai multe thread-uri?
28. Cum se face un obiect thread-safe in Java?
29. Ce este un keyword in Java?
30. Ce este final keyword?
31. Ce este static keyword?
32. Descrie cele 4 concepte POO.
33. Descrie SOLID Principles , cu exemple reale , in aplicatii Java
34. Care este diferenta dintre & si && in Java?
35. Care e diferenta dintre static synchronized si synchronized?
36. Cum fac o lista imutabila in Java?
37. Descrie Design Pattern-ul Builder
38. Descrie Design Pattern-ul Facade
39. Care e diferenta dintre Abstract Factory Design Pattern si Factory Design Pattern? Descrie-le. ref: https://www.baeldung.com/cs/factory-method-vs-factory-vs-abstract-factory
40. Care sunt modificatorii de acces in Java? Descrie
41. Ce face o clasa final in Java?
42. Intr-o clasa abstracta, putem avea metode neabstracte? Dar invers?
43. Descrie agregarea si compozitia
44. Cate clase publice putem avea intr-un fisier .java?
45. Care este lifecycle ul unui thread in Java? ref: https://www.baeldung.com/java-thread-lifecycle
46. In general de stream-uri, operatii intermediare si finale, exemple.
47. Ce este un pachet in Java? Ce este un modul in Java?
48. Despre Consumer, Supplier, Function si Predicate. Cum putem face o lambda function in Java?
49. Avem nevoie neaparat de adnotarea de FunctionInterface pentru a face o interfata sa fie functionala?
50. Daca extindem o interfata, toate metodele trebuie sa fie implementate? Dar daca avem o clasa abstracta, trebuie toate metodele sa fie implementate?
51. Comparable vs Comparator
52. Intr-un enum putem avea metode abstracte? Daca da, cum si ce fac?
53. Pattern matching, variabila este 'final'.
54. Ce modificatori de acces este implicit pentru metode in interfete? 
55. In java cate clase putem extinde in mostenire? Dar cate putem implementa?
56. Diferenta dintre stream.toList() si stream.collect(Collectors.toList()) -> imutabilitate / mutabilitate
57. Care e diferenta dintre un thread si un proces?
58. Care e diferenta dintre programare reactiva si programare concurenta?
59. Complexitati la Collections (la cam toate) si care e thread-safe si care nu.
60. Despre o structura de date care are complexitatea de cautare O(log n).
61. Despre semaphores, mutex-uri
62. Cum se face resize-ul la un Arraylist? - Despre load factor si capacity. by default, se face x2 cand se atinge load factor-ul.
63. 'have you used other communications than REST in your projects?'
64. 'how hashcode and equals work in a hashmap?'
65. 'is hashmap thread-safe? tell us a thread-safe data structure for hashmap. what's the difference between Collections.synchronizedMap vs. ConcurrentHashMap?'
66. 'what is the difference between a process, a thread and a coroutine? -> kotlin'
67. Se poate folosi urmatorul scenariu? Cand?:
```java
try {

} catch (T t) {

}
```
68. Poti seta thread pools la un parallel stream? Cum?
69. Ce inseamna ca un obiect este serializabil? Cum faci un obiect serializabil? Vorbeste despre serialVersionUID si pentru ce se foloseste.
70. Ce este un 'pure function'? Cum te poti folosi de o clasa imutabila pentru a realiza un pure function?
71. Pentru ce se foloseste volatile?
72. Pe ce putem folosi synchronized?
73. Care e diferenta dintre Runnable si Callable?
74. Functions de genul (denumire):
```java
public void f1() {
    f2(d -> d.equals("e"));
}
        
private void f2(Function<Object, Object> f) {
    
}
```
75. Cand o resursa poate fi folosita cu try-with-resources? ce trebuie sa implementeze?
76. Care sunt cele 3 tipuri de design patterns ?
77. Ai folosi streams cand ai operatii CPU intensive sau I/O intensive? 
78. 'what's the difference between strategy and state patterns?'
79. 'what is the reason of static methods? what is an utility class? what's the difference between using an interface and a class when we build an utility class?'
80. 'why and when to use default methods in interfaces?'
81. 'what's the lifecycle of maven?'
82. 'have you used maven as parent with modules?'
83. vorbeste despre stream-uri (orice, finite/infinite, stream-uri normale si parallel streams). modalitatea de cum functioneaza un parallel stream -> forkjoin method
84. vorbeste despre lock, cand se foloseste, un exemplu cand poti sa obtii deadlock si cum ai rezolva daca ai avea un deadlock in productie? -> thread dumps

##### Coding / Clean Code
1. Construieste un cache de mana -> folosind HashMap. Ce se intampla daca folosim un Key de tip Object cu 2 field-uri, cu getters si setters si folosesc cheia respectiva si dupa aceea schimb un field. Se schimba hashcode-ul din hashmap? Cum se face key-ul imutabil?

Concret:
```java
public class KeyObject {
    private String field1;
    private String field2;
    // getters, setters, constructor etc.
}

public class TestClass {
    private final Map<KeyObject, CustomObject> customCache = new HashMap<>();
    
    public void method1() {
        KeyObject key1 = new KeyObject("f1", "f2");
        customCache.put(key1, new CustomObject());
        
        // what happens? how to fix?
        key1.setField1("f3");
    }
}
```

2. Cum rezolvam daca avem 2 query-uri incapsulate si pica unul din ele si vrem sa facem rollback?

Concret:
```java
@Service
class MyService {

 

    Dao1 dao1;
    Dao2 dao2;

    
    // Here, add @Transactional.
    public void m1() {

        dao1.save();
        dao2.save();
    }
}
```

Sa presupunem ca adaugam o metoda m2() la implementarea de sus. Ce se intampla daca nu adaugam @Transactional pe ea?

3. Transforma metoda urmatoare in cod functional:
```java
public class FunctionalClass {
    
    public Integer func(Map<String, List<Integer>> map) {
        for (var values : map.values()) {
            for (var values2 : values) {
                if (10 == values2) {
                    return values2 * 10;
                }
            }
        }
        
        throw new RuntimeException();
        
        return null;
    }
}
```
Hint: flatmap, filter, map.

4. Problema de code review ce continea .close() fara try-with-resources. Negari prima data si conditii in cod (tratare cazuri), simplificare cerinta de code loading si exception code.
5. Explica care este problema daca am pasa intr-o metoda 9 argumente si cum poti rezolva asta? De ce este o problema de clean code sa pasam intr-o metoda 3 parametrii booleni, de exemplu: 'true, true, false'. Cum poti rezolva asta? -> clean code/uncle bob, enums


# Spring / API
1. Se da metoda getById din Hibernate care are 'foarte multe cereri'. Cum sporesti performanta? --> cacheable, cum faci o metoda sa fie cacheable in Spring
2. Cum se face health check la o aplicatie spring boot?
3. Sunt @Controller, @Service si @Repository bean-uri?
4. Bean-ul e singleton.
5. Cum initializam in spring test un @Bean? @MockBean si context - adnotare?
6. Cum adaugam bean-uri fara @Bean? @Component?
7. Diferenta dintre autentificare si autorizare.
8. De @RequestMapping
9. Diferenta dintre POST si PUT - idempotenta
10. Ce relatii exista? De @JoinColumn -> la ambele cazuri
11. Fetch type by default la @OneToMany, @ManyToMany, @OneToOne, @ManyToOne
12. Cum se triggeruiesc niste job-uri in Spring? -> Spring Batch, @Scheduler, 
13. Cum functioneaza Spring Batch? -> Reader, Writer, Processor, Job, JobLauncher
14. Spring Profiles
15. Spring MVC, Tomcat, blocant, 1 thread per request
16. Descrie @Transactional. Spune despre izolare si despre propagare
17. De @Qualifier
18. Comunicare microservicii -> variante posibile, descriere din proiecte (WebClient/Feign Client/JMS-uri)
19. n+1 query problem. Cum scapi de ea?
20. Cum functioneaza proxy-urile in Hibernate? (la fetch type cum se populeaza)
21. Despre tot flow-ul de la Controller la Repository. (@Entity, @Column, @Table, @Service, @Repository, @Controller/@RestController)
22. Care e diferenta dintre @Controller si @RestController?
23. Ce face @Autowired?
24. De @ConfigurationProperties
25. Cum definesti o metoda in spring ca fiind una de test?'
26. 'what's the difference between spring boot 2 and spring boot 3, what we're the challenges?'
27. 'what are unit tests and integration tests? how you wrote them?'
28. Ce module din spring ai folosit?
29. Inafara de singleton, ce scope-uri mai are un bean?
30. Daca vreau sa folosesc mai multe instante inloc de una la un bean, cum pot face asta?
31. Unde se poate folosi @Autowired?
32. Daca ar fi sa folosesti @Autowired, ai folosi pe constructor sau pe field-uri? Care sunt cazurile cand se foloseste pe field-uri?
33. Care este flow-ul de security? Povesteste de la inceputul request-ului pana la implementare, ceea ce se intampla in spate.
34. De la ce vine csrf? De la ce vine cors? Cu ce ne ajuta cors? Cu ce ne ajuta csrf?
35. Spring promoveaza mai mult agregarea sau compozitia? Ce ai folosi mai mult? -> exemple SOLID
36. Cum se configureaza Vault? Spring stocheaza datele din Vault?
37. Ce face Spring actuator?
38. Care este prefixul pentru JWT Token? Cum folosesti JWT Token? Care este structura JWT Token? Cum validezi un JWT Token?
39. Folosesti OAuth2 sau Basic Auth? Cum functioneaza ambele?
40. Cum faci partea de testare? Ai aplicat vreodata TDD principles? Care sunt beneficiile TDD?
41. Cum stochezi un token? Le salvati in baza de date? E de ajuns sa fie validate? Ce folositi ca validator?
42. Ce e un topic? -> JMS
43. Ce folosesti pentru testele de integrare? Cum le faci?
44. Cum salvezi in local storage un token?
45. Cum folosesti cookies?
46. Descrie SSL Handshake.
47. Despre LDAP???
48. 'difference between interceptor and filter'
49. 'have you ever tested a static method?'
50. 'have you ever used @Primary? when you use this annotation?'
51. 'how is configuration done in spring boot?'
52. 'what's the difference between spring and spring boot?'
53. 'how do you connect to multiple databases in spring boot? have you ever used jpa without hibernate?'
54. care e diferenta dintre java singleton si spring singleton?
55. ce face bean scope session? exemplu real cand am putea sa-l folosim? care este lifecycle-ul?
56. cum faceati handle la spring security la operatia de delete daca foloseati OAuth2?
57. cum functioneaza mai exact spring proxies? -> vorbeste despre cum functioneaza proxy-urile daca ai un service care implementeaza o interfata si cand nu. (in spate)
58. sa presupunem ca ai doua tranzactii, in aceeasi clasa, una cu @Transactional si una cu @Transactional, dar cu propagarea requires_new. cate tranzactii sunt facute? dar cand folosesti metodele in clase diferite, cate sunt?
 
### Data Structures & Algorithms
1. https://leetcode.com/problems/range-sum-of-bst/ -> bts range sum
2. https://leetcode.com/problems/two-sum/ -> two sum
3. https://leetcode.com/problems/implement-queue-using-stacks/ -> 2 stacks for queue
4. https://leetcode.com/problems/implement-stack-using-queues/ -> 2 queues for stack

### SQL & NoSQL
1. Se dau doua tabele: studenti si profesori, iar un profesor preda mai multe materii. Descrie tipul de relatie si proiecteaza tabelele. Afla top 3 cei mai populari profesori dupa numarul de studenti inscrisi la cursuri.
2. La ce se foloseste un index? Care e diferenta dintre un index btree si index bitmap? Care e problema daca folosim un index bitmap? -> probleme performanta la insert
3. Normalizare si denormalizare.
4. CAP Theorem
5. 'what you mean with MongoDB is more scalable?' when you used it?
6. 'what are the 2 letters from CAP that mongodb have?'
7. Cand folosim indecsi? Cand se foloseste un index bitmap?
8. cate tipuri de indecsi sunt? foreign key este un index?
9. explica ce date sunt luate la un left outer join
10. in general, care este rolul unei tranzactii?
11. cate tipuri de view-uri exista? ai auzit despre view-uri materializate?
12. Ai auzit de database pages? Poti descrie ce fac/ce sunt?

### DevOps
1. Spring Profiles -> Kubernetes ConfigMaps
2. Ce este un replica set?
3. Ce este un deployment?
4. Care e diferenta dintre docker si o masina virtuala? -> kernel?
5. Cum poti afla informatii despre resurse in SO linux? -> top/htop?
6. Cum pornesti un serviciu in linux? -> systemctl, systemd
7. Despre cd, ls, grep.
8. 'tell us more about api gateway, what is an api gateway?'
9. 'what is docker and docker-compose?'
10. 'what is sonarqube? how have you used it?'
11. Care e diferenta dintre http si https?
12. Cum se pot conecta doua containere de docker intre ele?
13. Daca vrem sa persistam datele, ce ai folosi? -> docker volumes
14. Ai folosit vreodata nginx? Pentru ce se foloseste?
15. Ce este prometheus? Apeleaza endpoint-urile de spring sau nu? La ce se foloseste?
16. La ce se foloseste Vault?
17. De la ce vine ACID?
18. De ce ai nevoie ca un http sa fie securizat?
19. 'what is DOS and DDOS?'
20. 'tell me about Log4j vulnerability, what happened?'
21. 'what's the difference between a docker image and docker container?'

### Microservices , Distributed Apps?
1. 'what are the properties of a microservice?' -> Reliable, Scalable, and Maintainable. -> dupa business logic si baza de date independenta
2. 'what are the pitfalls of using microservices?'
3. 'tell me about quality attributes'
4. 'what are the benefits of using microservice architecture?'
5. 'microservice vs serverless'

### Agile & SCRUM
1. 'do you work SCRUM? how does is work for your team?'
2. tell us how you work scrum? (about daily, retro, etc.)


### System Design
1. Explica cache, cand se foloseste, cum faci cache, de cache-uiesti, despre eviction policies
2. Sa presupunem ca ai o echipa care pe moment decide sa construiasca o aplicatie care e un monolit, dar pe viitor doreste sa migreze la microservcii. cum ar arata aplicatia respectiva?
3. care este diferenta dintre comunicare sincrona si asincrona?
4. avand in vedere proiectul explicat, cum ai putea sa-l imbunatatesti?
5. care sunt beneficiile folosind un sistem distribuit?
6. despre ce este vorba la hexagonal architecture?
7. cum poti sa faci o comunicare asicrona folosind http 1?
8. sa presupunem ca ai vrea sa construiesti un API REST care creeaza masini virtuale si sa presupunem ca sistemul funtioneaza in felul urmator: in cazul in care vrei sa creezi o masina virtuala, acest proces dureaza in jur de 20-25 minute. In cazul in care faci o cerere, aceasta sa fie inregistrata si sa presupunem ca ai un numar limita de 50 de masini virtuale spre exemplu care pot fi create simultan. Cum ai face design-ul (request body + response body) la un astfel de sistem? -> de aici porneau mai multe intrebari in legatura cu status code, design, reguli si proprietati REST (fara sa implica Spring) si o intrebare despre cum am face un endpoint care sa returneze doua response body-uri diferite fara a schimba numele endpoint-ului.
