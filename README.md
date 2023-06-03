# crack-bucharest-interviews
Intrebari si probleme pe care le-am primit pana acum la interviuri. (Java Developer)

# Java Vanilla / Generale

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

##### Coding
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
19. n+1 query problem
20. Cum functioneaza proxy-urile in Hibernate? (la fetch type cum se populeaza)

# Data Structures & Algorithms
1. https://leetcode.com/problems/range-sum-of-bst/ -> bts range sum
2. https://leetcode.com/problems/two-sum/ -> two sum
3. https://leetcode.com/problems/implement-queue-using-stacks/ -> 2 stacks for queue
4. https://leetcode.com/problems/implement-stack-using-queues/ -> 2 queues for stack

# SQL
1. Se dau doua tabele: studenti si profesori, iar un profesor preda mai multe materii. Descrie tipul de relatie si proiecteaza tabelele. Afla top 3 cei mai populari profesori dupa numarul de studenti inscrisi la cursuri.
2. La ce se foloseste un index? Care e diferenta dintre un index btree si index bitmap? Care e problema daca folosim un index bitmap? -> probleme performanta la insert
3. Normalizare si denormalizare.
4. CAP Theorem

# DevOps
1. Spring Profiles -> Kubernetes ConfigMaps
2. Ce este un replica set?
3. Ce este un deployment?
4. Care e diferenta dintre docker si o masina virtuala? -> kernel?
5. Cum poti afla informatii despre resurse in SO linux? -> top/htop?
6. Cum pornesti un serviciu in linux? -> systemctl, systemd
7. Despre cd, ls, grep.