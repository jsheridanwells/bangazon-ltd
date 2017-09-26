# Workforce Asset and Training Application

## Table of Contents

1. [Prerequisites](#prerequisites)
1. [What You Will Be Learning](#what-you-will-be-learning)
1. [Requirements](#requirements)
1. [Resources](#resources)

## Prerequisites

* [ASP.NET MVC](https://docs.asp.net/en/latest/mvc/overview.html)
* Migrations
* [View templates/Layouts](https://docs.asp.net/en/latest/mvc/views/overview.html)
* Forms
* Controllers
* ERD development
* Routing
* Yeoman, and the ASP.NET generator, [installed](#installing-yeoman-and-the-aspnet-generator)

## What You Will Be Learning

### Server Generated Application

All views in this application will be generated on the server, using templates, and delivered to the client as a complete HTML document.

### View Templates

You learned about view templates when you used Angular, but now your application server will be serving a fully built template to any client request instead of the client building the view.

### Layouts

To keep your code DRY between different view templates, you should use a [layout](https://docs.asp.net/en/latest/mvc/views/layout.html) to define the general structure of your site, and the individual page templates will be injected into the overall layout.

### Forms

The ASP.NET MVC framework provides many conventions and helpers that make building forms easier, and are bound to view models, much the same way that you used Angular to bind form fields in a partial to variables and/or objects in a controller.

## Requirements

You will be building a fairly straightforward, server generated MVC application for performing CRUD operations on the following resources:

* Employees
* Departments
* Computers
* Training Programs

The following relationships must be established.

1. Over time, a computer can belong to many employees, but only one at a time.
1. An employee can attend many training programs.
1. A training program can have many employees attending.
1. Many employees can be assigned to a department, but an employees may only be in one at a time.

Produce the following views.

### Employee Views

1. List employees.
1. Create an employee, and assign to a department.
1. View employee, which shows their department, computer, and any training programs they are attending.
1. Edit employee, which should also allow the user to:
    1. Reassign the employee to a different department
    1. Change which computer they are using from a list of unused computers.
    1. Add and/or remove training programs that the employee is attending.

### Department Views

1. List departments.
1. Create a department.
1. Department details, which should show all employees in that department.

### Computer Views

1. List computers, and be able to delete a computer from the list view.
1. Create a computer.

### Training Program Views

1. List training programs.
1. Create training program.
1. View training program details. This should display any employees that are currently in the training program

### Common Views

1. Basic navigation bar that allows the user to view the list of each type of resource.
1. Footer containing the company name.

## Resources

### Razor Templates

ASP.NET MVC views are generated by the [Razor view engine](https://docs.asp.net/en/latest/mvc/overview.html#razor-view-engine). You will find them *very* similar to Handlebar templates that you used in the client side course of NSS.