Download Link: https://assignmentchef.com/product/solved-cis407a-week-1-ilab-annual-salary-calculator
<br>
<header class="entry-header">

 <h1 class="entry-title"><strong style="font-size: 16px;">iLAB OVERVIEW</strong></h1>

</header>

5/5 - (2 votes)

<strong>Scenario/Summary</strong>

In this iLab, you will create an Annual Salary Calculator ASP.NET web application using Visual Studio.NET 2008.For the iLabs, you will use the Microsoft Visual Studio 2008 software application. You have two options for using this application:

<ul>

 <li style="list-style-type: none;">

  <ul>

   <li>You may use a copy of Visual Studio 2008 that is installed on your local PC. If you do not already have this software, there is a link in the Syllabus (in the Textbook and Required Materials section) that you can follow to obtain a copy at low or no cost through the DeVry Student Software Fulfillment Center.</li>

  </ul></li>

</ul>

<strong>OR</strong>

<ul>

 <li>You may run Visual Studio 2008 over the Web from the DeVry iLab (Citrix) server. Instructions for using the iLab (Citrix) server are on the iLab page under Course Home.Throughout this course, you will be creating a web application for a fictitious company called CoolBiz Productions, Inc. To get familiar with the development environment, follow the Lab Steps to create a simpleAnnual Salary Calculator ASP.NET web application. You will be adding to this application each week.Instructions for Week 1 iLab: “Hello World, and more” ASP.NET Web Application</li>

</ul>

<strong>Overview of Fictitious Company</strong>CoolBiz Productions, Inc.We are a mid-size indie (independent) film studio that is in need of a payroll system. We have outgrown our current system, a simple spreadsheet, to the extent that it takes three people over one week to pay everyone on a timely basis.

<strong>Overview of Our Company</strong>We have over 2,000 full-time and part-time employees. We produce comedy, fiction, and science fiction films with budgets of $250K–$20 million. We have produced over 50 films since we first began 20 years ago.We are very profitable and have strong links to many of the industry’s most powerful people.

<strong>Current Payroll System</strong>Our current system consists of mostly manual processing using an MS Excel spreadsheet to control who gets paid.The system consists of the three payroll staff members reviewing each of the full-time staff members’ wages, calculating how many hours they worked based on their hourly rate, and paying them by issuing a check.The check needs to be entered in another worksheet for each of the people who were paid so that we can tell when it went out, how much it was for, and if it was cashed or not. If a [Date_Cashed] is entered, we deduct that amount from our working payroll capital account to track how much money we have for payroll.This process is then repeated for all part-time staff and independent contractors.

<strong>Our Needs</strong>We need a more automated way to pay our staff. We need to use the same logical flow as a basis, yet improve on it by having a way to

<ol type="1">

 <li>easily calculate the projected annual salary based on rate and number of hours;</li>

 <li>search, enter, update, and delete staff and independent employee information in one place;</li>

 <li>search, enter, update, and delete payroll automation information for the employee to set up recurring payments or one-time payments;</li>

 <li>produce reports to show the following: (a) summary of who got paid per week, (b) summary of all payments per week, (c) details of any employee to-date (allow entry of a specific employee ID);</li>

 <li>allow transactions to be rolled back in case we pay someone too much;</li>

 <li>make use of transaction processing in case the system unexpectedly shuts down;</li>

 <li>ensure the system is secure (logins required);</li>

 <li>allow only authorized payroll personnel to control all aspects of the system;</li>

 <li>allow only authorized payroll personnel to view transactions and user activity;</li>

 <li>allow only authorized payroll personnel to e-mail reports to users using the e-mail on file; and</li>

 <li>incorporate error handling into all processes in the system and e-mail any errors to the technical support people.</li>

</ol>

<strong>Deliverables</strong>All files are located in the subdirectory of the website. The website should function as follows: You should have a page that, when run, displays a page showing the text “Hello, World.” You should also have a second page that is the annual salary calculator that properly calculates the annual salary, given an hourly rate and the number of hours projected to be worked in a year. Once you have verified both pages work, save your website, zip up all files, and submit in the Dropbox.

<strong>iLAB STEPS</strong>

In this ilab, we will learn how to create a simple ASP.NET web application using Microsoft Visual Studio.NET 2008. The application will display the text “Hello, World” on the home page.

<ol type="1">

 <li>Open Microsoft Visual Studio 2008.</li>

 <li>Create a new ASP.NET website called “PayrollSystem.” To do this, select “File, New Website.”When the “New Website” dialog opens, select “ASP.NET Website” as the Template, select “File System” as the Location, and select “Visual C#” as the Language. Click Browse and navigate to the folder where you want to save your website. Add “PayrollSystem” at the end of the file path. Click OK if you are prompted to create a new folder. Click OK in the New Website dialog to finish creating the website.</li>

 <li>Edit the Default.aspx file (the home page for your site) to add the message “Hello, World.” To do this, if necessary, click the Design button below the editing window to switch to Design view, then click in the editing window and type “Hello, World” (without the quotes).Click the Save button on the toolbar to save the changes to Default.aspx.</li>

 <li>To ensure that everything is working properly, click the Start Debugging button on the toolbar, or press the F5 key on the keyboard, or pull down the Debug menu and select “Start Debugging.”</li>

 <li>If the “Debugging Not Enabled” dialog box appears, select the option to add or modify the Web.config file to enable debugging and click OK. You should only have to do this the first time you debug the site.<em>NOTE:</em> To execute the application, you have these options:

  <ul>

   <li>If you are using Citrix, press CTRL + F5 to Start Without Debugging. You will not be deducted points for this part.</li>

   <li>If you are using a standalone version, press F5 to Start with Debugging, or you can press CTRL + F5 to Start Without Debugging</li>

  </ul></li>

 <li>The Internet Explorer web browser will open and display your Default.aspx page containing the “Hello, World” message.</li>

 <li>Click here for text description of this image.</li>

 <li>Stop debugging and return to the design mode by closing the browser.</li>

 <li>Add a new form to your web application called frmSalaryCalculator.aspx. Make sure “Place Code in separate file” is checked when you add the form. To add a new form, click (single-click, not double-click) on the project node in the solution explorer.With the project node highlighted, right-click on the project node and select “Add New Item” from the popup menu. The following dialog will be displayed:Select the name of the form you will add frmSalaryCalculator.aspx. Make sure “Place code in separate file” is checked and “Select master page” is unchecked.</li>

 <li>You will create a web-based salary calculator on this new page. To do this, open the aspx page in Design view and, from the Toolbox, add three labels, two text box controls, and a button control. You can add controls by dragging the control from the Toolbox – Standard section onto your form. Your form should look like this:</li>

 <li>Change the text displayed in each label so that the first label displays “Annual Hours”; the second label should display “Rate” and the third label should display “$”. (Hint: To change the text displayed, change the Text property of each control.)</li>

 <li>Change the button text to display “Calculate Salary.” (Hint: To change the text displayed as the button label, change the Text property of the button.) Your form should now look like this:</li>

 <li>Set the ID property of the top text box to txtAnnualHours. Set the ID property of the second textbox to txtRate. Set the ID of the bottom label (the one we set the text property to “$”) to lblSalary. (Note: We set these IDs as we will be accessing the control values from the C# code. You can set the button ID and the other two labels’ ID properties as well, but we won’t be accessing them from our code.)</li>

 <li>In Design view, add a C# event handler for the button-click event by double-clicking on the Calculate Salary button. This will place you in the page code behind file the editor. (Remember that ASP.Net pages have a file containing the HTML markup with an extension of .aspx and a C# ‘code behind’ file with an extension of .aspx.cs.) This is the code that should be displayed: (If you changed the ID of the button, it will be a different method name.)This code will be called each time the user presses the button. It is important to remember that code in the code behind page executes on the server – not on the user’s browser. This means that when the button is pressed, the page is submitted back to the web server and is processed by the ASP.Net application server on the web server. It is this code (between the { and } in this method) that will execute on the server. Once it is done executing the page will be sent back to the browser. Any changes we make to the page or controls on the page will be shown to the user in the updated page.</li>

 <li>In this method, add code that will get the text in the txtAnnualHours text box, convert it to a Double, and store it in a double variable. Add code that will get the text from the txtRate text box, convert it to a Double, and store it in another variable. Create a third variable of type Double and set its value to the annual hours variable value multiplied by the rate double variable value. Take this resulting value and convert it to a string (text), and update the lblSalary Text property with this new string.<strong>Hints:</strong> A control’s property can be accessed by simply using the control ID followed by a . followed by the name of the property. For example, the value stored in the Text property of the txtAnnualHours control can be accessed by using this: txtAnnualHours.Text. Text properties on controls are of type string.To convert a string to a Double you can use the Convert class. If we had a string variable called str1 and a double variable called myNumber, the C# code to convert this would be as follows:When converting from one type to another, we are assuming that the value stored in the type being converted is compatible with the type we are converting to. In the example above, if the value stored in str1 was not type compatible with a Double (for example “tiger”) an error would be raised.To set the value of a control on a web form, you can access the control and set the property directly. If I had a label control called lblCar and I wanted to update the text that was displayed in the label, I could do something like this:Note that following code would be incorrect and cause an error:lblCar is a Label – it isn’t a string so we can’t assign a string directly to it, but we can assign a string directly to the Text property of the label.All of the base types in C# (double, int etc) have a ToString() method you can call. If you had a double variable that you wanted to convert to a string and set that string to my label’s text, you would do the following:This would take whatever value was stored in the myNumber Double and convert it to a string.To add a $ to output you can use string concatenation in C# like this:</li>

 <li>Set your new form as the start page by clicking once on the form name in the Solution Explorer and then right-clicking on the form name and selecting “Set as Start Page.” You can now test your application and make sure it works correctly as you did with the Hello World form above. You can switch back and forth between which form runs when you run your application by setting the different forms as the start page.</li>

</ol>