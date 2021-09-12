# **REST**
Consuming REST APIs in a React Application can be done in various ways, but in this tutorial, we will be discussing how we can consume REST APIs using two of the most popular methods known as Axios (a promise-based HTTP client) and Fetch API (a browser in-built web API). I will discuss and implement each of these methods in detail and shed light on some of the cool features each of them have to offer.

APIs are what we can use to supercharge our React applications with data. There are certain operations that can’t be done on the client-side, so these operations are implemented on the server-side. We can then use the APIs to consume the data on the client-side.

APIs consist of a set of data, that is often in JSON format with specified endpoints. When we access data from an API, we want to access specific endpoints within that API framework. We can also say that an API is a contractual agreement between two services over the shape of request and response. The code is just a byproduct. It also contains the terms of this data exchange.

In React, there are various ways we can consume REST APIs in our applications, these ways include using the JavaScript inbuilt fetch() method and Axios which is a promise-based HTTP client for the browser and Node.js.

Note: A good knowledge of ReactJS, React Hooks, JavaScript and CSS will come in handy as you work your way throughout this tutorial.

Let’s get started with learning more about the REST API.

his tutorial shows a collection of apps that use Spring Data REST and its powerful backend functionality, combined with React’s sophisticated features to build an easy-to-understand UI.

* Spring Data REST provides a fast way to build hypermedia-powered repositories.

* React is Facebook’s solution to efficient, fast, and easy-to-use views in JavaScript.

### **Part 1 — Basic Features**
This section shows how to get a bare-bones Spring Data REST application up and running quickly. Then it shows how to build a simple UI on top of it by using Facebook’s React.js toolset.
### **Step 0 — Setting up Your Environment**
Feel free to grab the code from this repository and follow along.

If you want to do it yourself, visit https://start.spring.io and pick the following dependencies:

* Rest Repositories

* Thymeleaf

* JPA

* H2
```
@Entity (1)
public class Employee {

	private @Id @GeneratedValue Long id; (2)
	private String firstName;
	private String lastName;
	private String description;

	private Employee() {}

	public Employee(String firstName, String lastName, String description) {
		this.firstName = firstName;
		this.lastName = lastName;
		this.description = description;
	}

	@Override
	public boolean equals(Object o) {
		if (this == o) return true;
		if (o == null || getClass() != o.getClass()) return false;
		Employee employee = (Employee) o;
		return Objects.equals(id, employee.id) &&
			Objects.equals(firstName, employee.firstName) &&
			Objects.equals(lastName, employee.lastName) &&
			Objects.equals(description, employee.description);
	}

	@Override
	public int hashCode() {

		return Objects.hash(id, firstName, lastName, description);
	}

	public Long getId() {
		return id;
	}

	public void setId(Long id) {
		this.id = id;
	}

	public String getFirstName() {
		return firstName;
	}

	public void setFirstName(String firstName) {
		this.firstName = firstName;
	}

	public String getLastName() {
		return lastName;
	}

	public void setLastName(String lastName) {
		this.lastName = lastName;
	}

	public String getDescription() {
		return description;
	}

	public void setDescription(String description) {
		this.description = description;
	}

	@Override
	public String toString() {
		return "Employee{" +
			"id=" + id +
			", firstName='" + firstName + '\'' +
			", lastName='" + lastName + '\'' +
			", description='" + description + '\'' +
			'}';
	}
}
```
![](https://i.ytimg.com/vi/ieMhlyjPjWo/maxresdefault.jpg)
