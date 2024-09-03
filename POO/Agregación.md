Hablamos de aquellas clases que tienen una relación con otra, pero que no son dependientes una de la otra. Es decir, si una clase desaparece, la otra sigue funcionando a diferencia de la [[Composición|composición]].

La agregación te puede servir para reutilizar código y no repetirlo.

Ejemplo:

Address.java
1. `public class Address {`  
2. `String city,state,country;`  

4. `public Address(String city, String state, String country) {`  
5.     `this.city = city;`  
6.     `this.state = state;`  
7.     `this.country = country;`  
8. `}`  

10. `}`

Emp.java
1. `public class Emp {`  
2. `int id;`  
3. `String name;`  
4. `Address address;`  

6. `public Emp(int id, String name,Address address) {`  
7.     `this.id = id;`  
8.     `this.name = name;`  
9.     `this.address=address;`  
10. `}`  

12. `void display(){`  
13. `System.out.println(id+" "+name);`  
14. `System.out.println(address.city+" "+address.state+" "+address.country);`  
15. `}`  

17. `public static void main(String[] args) {`  
18. `Address address1=new Address("gzb","UP","india");`  
19. `Address address2=new Address("gno","UP","india");`  

21. `Emp e=new Emp(111,"varun",address1);`  
22. `Emp e2=new Emp(112,"arun",address2);`  

24. `e.display();`  
25. `e2.display();`  

27. `}`  
28. `}`