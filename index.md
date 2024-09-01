# Welcome to My Markdown File
## Introduction
### to markdown
#### skills communicate



Added H1 ,H2 ,H3 and H2 headers to index.md

![Iron Man](https://i.pinimg.com/originals/cb/30/8e/cb308eb09c9e592e545984a5ef16c464.jpg)

- [ ] Open GitHub Pages
- [ ] Show my portfolio
- [ ] Introduce myself to the world

```javascript
import java.util.Scanner;
public class Inheritance
{
	public static void main(String[]args)
	{
		Scanner m = new Scanner(System.in);
		System.out.println("Employees : ");
		System.out.println("1. Officer ");
		System.out.println("2. Manager ");
		System.out.print("Enter your choice : ");
		int ch = m.nextInt();
		if(ch==1)
		{
			System.out.print("Enter officer name : ");
			String name = m.next();
			System.out.print("Enter officer age : ");
			int age = m.nextInt();
			System.out.print("Enter officer phone number : ");
			long phone = m.nextLong();
			System.out.print("Enter officer address : ");
			String address = m.next();
			System.out.print("Enter officer salary : ");
			double salary = m.nextDouble();
			System.out.print("Enter officer specialization : ");
			String specialization = m.next();
			Officer of = new Officer();
			of.details(name,age,phone,address,specialization);
			of.Salary(salary);
		}
		else if(ch==2)
		{
			System.out.print("Enter manager name : ");
			String name = m.next();
			System.out.print("Enter manager age : ");
			int age = m.nextInt();
			System.out.print("Enter officer phone number : ");
			long phone = m.nextLong();
			System.out.print("Enter manager address : ");
			String address = m.next();
			System.out.print("Enter manager salary : ");
			double salary = m.nextDouble();
			System.out.print("Enter manager department : ");
			String department = m.next();
			Manager ma = new Manager();
			ma.details(name,age,phone,address,department);
			ma.Salary(salary);
		}
		else
		{
			System.out.println("");
		}
	}
}
class Employee
{
	String name;
	int age;
	String address;
	double salary;
	void main(String name,int age,long phone,String address,double salary)
	{
		this.name = name;
		this.age = age;
		this.address = address;
		this.salary = salary;
		//this.phone = phone;
	}
	void Salary(double salary)
	{
		System.out.println("Salary : "+ salary);
	}
}
class Officer extends Employee
{
	String specialization;
	void details(String name,int age,long phone,String address,String specialization)
	{
		this.specialization = specialization;
		System.out.println("Name : "+ name);
		System.out.println("Age : "+ age);
		System.out.println("Phone number : "+ phone);
		System.out.println("Address : "+ address);
		System.out.println("Specialization : "+ specialization);
	}
	void Salary(double salary)
	{
		super.Salary(salary);
	}
}
class Manager extends Employee
{
	String department;
	void details(String name,int age,long phone,String address,String department)
	{
		this.department = department;
		System.out.println("Name : "+ name);
		System.out.println("Age : "+ age);
		System.out.println("Phone number : "+ phone);
		System.out.println("Address : "+ address);
		System.out.println("Department : "+ department);
	}
	void Salary(double salary)
	{
		super.Salary(salary);
	}
}
