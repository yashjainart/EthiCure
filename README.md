# ETHICURE - Your Heathhub Manager
Group Project-
Hospital Management System
Hospital Management System using MySQL, Php and Bootstrap


## Features to Implement:

1) Appointment Approval: Enable doctors to accept appointments and notify patients of approval.
2) Email Validation: Prevent users from registering with an already registered email ID.
3) Password Security: Ensure passwords are encrypted and not displayed in the admin panel.
4) Pagination: Implement pagination for all list views across the application.
5) Bug Fix - Bill Payment Receipt: Ensure the receipt does not contain multiple records for a patient associated with the same doctor multiple times.
6) Prescription Details: Add more fields to prescription statements for specificity.
7) Payment Details: Include additional details such as the date of payment and the amount paid.
8) Export Functionality: Add an export button in the admin module to export all details to an Excel sheet.

## Prerequisites
1. Install XAMPP web server
2. Any Editor 
3. Any web browser with latest version

## Languages and Technologies used
1. HTML5/CSS3
2. JavaScript (to create dynamically updating content)
3. Bootstrap (An HTML, CSS, and JS library)
4. XAMPP (A web server by Apache Friends)
5. PhP
6. MySQL (An RDBMS that uses SQL)
7. TCPDF (to generate PDFs)

## Steps to run the project in your machine
1. Download and install XAMPP in your machine
2. Clone or download the repository
3. Extract all the files and move it to the 'htdocs' folder of your XAMPP directory.
4. Start the Apache and Mysql in your XAMPP control panel.
5. Open your web browser and type 'localhost/phpmyadmin'
6. In phpmyadmin page, create a new database from the left panel and name it as 'myhmsdb'
7. Import the file 'myhmsdb.sql' inside your newly created database and click ok.
8. Open a new tab and type 'localhost/foldername' in the url of your browser

    
### SOFTWARES USED
  - XAMPP was installed on the Ubuntu 19.04 machine and APACHE2 Server and MySQL were initialized. And, files were built inside opt/lampp/htdocs/myhmsp
  - Sublime Text 3.2 was used as a text editor.
  - Google Chrome Version 77.0.3865.90 was used to run the project (localhost/myhmsp was used as the url).
  

### Starting Apache And MySQL in XAMPP:
  The XAMPP Control Panel allows you to manually start and stop Apache and MySQL. To start Apache or MySQL manually, click the ‘Start’ button under ‘Actions’.
  
  
![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/98f5d373-174c-4ccc-bff3-d479e758818b)


## GETTING INTO THE PROJECT:
The system includes a ‘Home’ page where patients, doctors, and administrators can log in to their accounts. Below is a visual guide to the system's main features and modules.


![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/7e564479-85bd-4961-b7dc-f906e88f7063)


'About Us' page allows us to get some more information about the quality and the services of the hospital.

![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/befbdfa2-5a16-4d82-a043-92efc88eabdd)

![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/9628633d-0ecc-4987-8c99-362e6fc1c76c)


‘Contact’ page allows users to provide feedback or queries about the services of the hospital. Fig below shows the ‘Contact’ page.

  ![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/d9d2320b-9458-464d-a30f-363e0d52a859)


The ‘Home’ page consists of 3 modules:
1. Patient Module
2. Doctor Module
3. Admin Module

### Patient Module:

  &nbsp; &nbsp; &nbsp; This module allows patients to create their account, book an appointment to see a doctor and see their appointment history.
  The registration page(in the home page itself) asks patients to enter their First Name, Last Name, Email ID, Contact Number, Password and radio buttons to select their gender.
  
  ![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/053a8cf0-174e-4ee1-9f5d-b6c270e983e1)


Once the patient has created his/her own account after clicking the ‘Register’ button, then he will be redirected to his/her Dashboard.

![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/6f36d28a-72f6-4477-9183-e4b08a56ea49)


The Dashboard page allows patients to perform two operations:

**1. Book his/her appointment:**

  &nbsp; &nbsp; &nbsp; Here, the patients can able to book their appointments to see a doctor. The appointment form requires patients to select the doctor that they want to see, Date and Time that they want to meet with the doctor. The consultancy fee will be shown accordingly to the patient as it was already determined by the doctor.

![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/2168cbc4-495b-415c-a9dd-2a6b040f5bce)


After clicking on the ‘Create new entry’ button, the patient will receive an alert that acknowledges the successful appointment of the patient.


**2. View patients’ Appointment History:**

  &nbsp; &nbsp; &nbsp; Here, the patient can see their appointment history which contains Doctor Name, Consultancy Fee, Appointment Date and Time.
	
![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/b22a862a-2b83-4de7-a1f8-9bdcabf02e74)


Once the patient has logged out of his account, if he wants to go into his account again, he can login his account, instead of register his account again. Fig below shows the login page.
Clicking on ‘Login’ button will redirect the patient to his dashboard page which we have seen earlier.

![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/7b311d7e-93ac-4b17-b402-833b18d7d1a5)


This is how the patient module works. On the whole, this module allows patients to register their account or login their account(if he/she has one), book an appointment and view his/her appointment history.

### Doctor Module:

  &nbsp; &nbsp; &nbsp; The doctors can login into their account which can be done by toggling the tab from ‘Patient’ to ‘Doctor’. Registration of a doctor account can be done only by admin. We will discuss more about this in Admin Module.
  
![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/c19ee6da-d17a-4419-b2ba-3c4b38badbfd)


Once the doctor clicking the ‘Login’ button, they will be redirected to their own dashboard.

![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/6b17dff6-c4e9-4296-880f-33f8ed24a6ac)


In this page, doctor can able to see their appointments which has been booked by the patients.

![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/49f1e3cd-5f62-4883-8757-f5bd7d3f1624)


In real-time, the doctors will have thousands of appointments. It will be easier for a doctor to search for appointment in the case of more appointments. To make it easier, I have a ‘Search’ box in the navigation bar which allows doctors to search for a patient by their contact number.
&nbsp; &nbsp; &nbsp; Once everything is done, the doctor can logout of their account. Thus, in general, a doctor can login into his/her account, view their appointments and search for a patient. This is all about Doctor Module.

### Admin Module:
   
   &nbsp; &nbsp; &nbsp; This module is the heart of our project where an admin can see the list of all patients. Doctors and appointments and the feedback/queries received from the ‘Contact’ page. Also admin can add doctor too. 
  &nbsp; &nbsp; &nbsp; Login into admin account can be done by toggling into admin tab of the Home page. 
  &nbsp; &nbsp; &nbsp; `username`: admin, `password`: admin123

![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/72089f59-9517-4288-b810-0e61faec26a5)


On clicking the ‘Login’ button, the admin will be redirected to his/her dashboard 

![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/d3f7203a-a62f-4961-9dd9-e70b15a60fd2)


This module allows admin to perform five major operations:

**1. View the list of all patients registered:**

  &nbsp; &nbsp; &nbsp; Admin can able to view all the patients registered. This includes the patients’ First Name, Last Name, Email ID, Contact Number and Password.As like in doctor module, admin can also search for a patient by their contact number in the search box.
  
  ![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/2eb1729f-7a4d-427f-8304-de742e7f9b43)

  
**2. View the list of all doctors registered:**

  &nbsp; &nbsp; &nbsp; Details of the doctors can also be viewed by the admin. This details include the Name of the doctor, Password, Email and Consultancy fees. Searching for a doctor can be done by using the doctor’s Email ID in the search box.

![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/ac9883fd-abd3-4a4a-acdd-adb77ee84bf7)


**3. View the Appointment lists:**

  &nbsp; &nbsp; &nbsp; Admin can also able to see the entire details of the appointment that shows the appointment details of the patients with their respective doctors. This includes the First Name, Last Name, Email and Contact Number of patients, doctor’s name, Appointment Date, Time and the Consultancy Fees. 

  ![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/94aa683f-3c17-4330-ae92-bea6e25178e5)

  
 **4. Add Doctor:**

  &nbsp; &nbsp; &nbsp; Admin alone can add a new doctor since anyone can register as a doctor if we put this section on the home page. This form asks Doctor’s Name, Email ID, Password and his/her Consultancy Fees.
  
  ![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/1606c6e0-bea7-4f6a-94f0-165fa0a4f499)

  
  After adding a new doctor, if we check the doctor’s list, we will see the details of new doctor is added to the list.
  
  ![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/508a7dac-8291-48b7-9c76-41b1dafe815b)

  
**5. View User’s feedback/Queries:**

  &nbsp; &nbsp; &nbsp; Admin is allowed to view the feedback/Query that has been given by the user in the ‘Contact’ page. This includes User’s Name, Email Id, Contact Number and the message(Feedback/ Query).
  
 ![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/87df262e-0a2f-44dc-bc3c-b5b5ecf16c13)

 **6. Delete Doctor:**

  &nbsp; &nbsp; &nbsp; Admin is allowed to Delete a previously added doctor.

  ![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/ea08a96d-c6b7-4093-84e3-bc16875e6fc8)

  After deleting a doctor we can see that he/she is removed from the doctor list.

  **7. View Prescription List for User:**

  &nbsp; &nbsp; &nbsp; Admin is allowed to view the Prescription List that has been given to the user by the doctor. 

  ![image](https://github.com/Kshitijboi/Ethicure/assets/116621388/ff6720a8-7f21-461e-85e3-8d96fc67179b)



  &nbsp; &nbsp; &nbsp; Taking everything into consideration, admin can able to view the details of patients and doctors, appointment details, Feedback by the user, add a new doctor, delete an existing doctor and 
  checking the Prescription List. Once everything is done, the admin can logout from his account.

  ** This was Ethicure Your Personal HealthHub Manager which manages everything related to your medication.**






