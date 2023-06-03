# crack-bucharest-interviews
Intrebari si probleme pe care le-am primit pana acum la interviuri. (Java Developer)

# Java Vanilla

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


# Spring
1. Se da metoda getById din Hibernate care are 'foarte multe cereri'. Cum sporesti performanta? --> cacheable, cum faci o metoda sa fie cacheable in Spring


# SQL
1. Se dau doua tabele: studenti si profesori, iar un profesor preda mai multe materii. Descrie tipul de relatie si proiecteaza tabelele. Afla top 3 cei mai populari profesori dupa numarul de studenti inscrisi la cursuri.