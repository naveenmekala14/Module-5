# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
~~~
# Python program for Hierarchical Inheritance

# Base class
class Details:

    def getName(self, name):
        self.name = name

    def getAge(self, age):
        self.age = age


# Derived class 1
class Employee(Details):

    def getEmployeeDetails(self, employee_id, department):
        self.employee_id = employee_id
        self.department = department

    def displayEmployee(self):
        print("\nEmployee Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Employee ID:", self.employee_id)
        print("Department:", self.department)


# Derived class 2
class Patient(Details):

    def getPatientDetails(self, patient_id, disease):
        self.patient_id = patient_id
        self.disease = disease

    def displayPatient(self):
        print("\nPatient Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)


# Employee object
emp = Employee()

ename = input("Enter Employee Name: ")
eage = int(input("Enter Employee Age: "))
eid = input("Enter Employee ID: ")
dept = input("Enter Department: ")

emp.getName(ename)
emp.getAge(eage)
emp.getEmployeeDetails(eid, dept)

# Patient object
pat = Patient()

pname = input("\nEnter Patient Name: ")
page = int(input("Enter Patient Age: "))
pid = input("Enter Patient ID: ")
disease = input("Enter Disease: ")

pat.getName(pname)
pat.getAge(page)
pat.getPatientDetails(pid, disease)

# Display details
emp.displayEmployee()
pat.displayPatient()
~~~
## Sample Output
~~~
Enter Employee Name: Arun
Enter Employee Age: 30
Enter Employee ID: E101
Enter Department: HR

Enter Patient Name: Ravi
Enter Patient Age: 25
Enter Patient ID: P201
Enter Disease: Fever

Employee Details
Name: Arun
Age: 30
Employee ID: E101
Department: HR

Patient Details
Name: Ravi
Age: 25
Patient ID: P201
Disease: Fever
~~~
# Result
The program is verified.


