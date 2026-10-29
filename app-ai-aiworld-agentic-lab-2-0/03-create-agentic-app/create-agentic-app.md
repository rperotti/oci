# Creating an Agentic Application and Test it

## Introduction

In this section we will take the workflow that we created in the two previous labs and add it to an agentic application.</br>
Estimated Time: 15 minutes

### Objectives

Understand the how to create a basic agent application.

### Usage Notes

   [](include:initial_hints)

## Task 1: Create the Agentic Application
1. From AI Agent home page on the left hand pane, select **Applications**.  When the application window, opens, select **Add**.</br>
![Add a new Application](images/create_the_app.png " ")
For the name of the applications use:  ***Your Initials*** and include **AI World Agentic Webinar Application**</br>
You can copy the workflow name by copying it here.
   ```txt
   <copy>
   AI World Agentic Webinar Application
   </copy>
   ```
Description: ***Copy the application name***
Press **Create** when you have provided  the name and description.
![Locate Your Workflow](images/use_initials_to_copy.png " ")
2. Add a new section to the application and add your workflow</br>
We will now add a new section to the agentic application and add our published workflow to it.</br>
Click on **Add Section**.

![Add a New Section](images/add_section_again.png " ")
Search for your workflow to add to the section.  Use the initials that you used to locate your workflow.</br>
If your workflow doesn’t show up you may need to check to make sure you published it or you didn’t set the **Agentic Apps** switch when creating it.</br>
![Add Your Workflow](images/add_workflow.png " ")
3. Name the Panel</br>
Click on the default panel name.  Then click on the Pencil icon to the right.</br>
You can use the name provided here or give it a name of your own.</br>
Name: **Pre-built workflow that will return all open requisitions with their status**</br>
When you have entered the panel name, click on the **Check box** to the right of the panel.
![Name the New Section](images/name_pane_1.png " ")

## Task 2: Run the Agentic Application
1. Run the application
To run the application, click on the **Play** button on the menu at the bottom of the page.<br>
![Run the Application](images/run_the_app.png " ")

2. Observe the Output</br>
When this section of the workflow is executed, your workflow is executed.  The following actions happen.</br></br>
1- The workflow is loaded and the **InitDisplay** is passed into the workflow.</br>
2- The agent step calls the **AI World Retrieve All Requisition** agent.</br>
3- The agent queries the Purchase Requisition business object and returns the requested requisition information.</br>
4- For each requisition line, The agent calls the external REST end point **Supplier Inquiry** that will return the inventory count for the line item.<br>
5- Once complete, the agent node is complete. The LLM node is executed next. The LLM will format the data.</br>
6- For any inventory item that is zero, it will set the output text to include a **oraInsight** message and a **oraComms** message.<br>
   (this was displayed in the debug in the previous lab)</br>
7- When the LLM step is done, the output text is passed back to the agentic app and displayed in the application.</br>
![Observe the Output](images/observe_output.png " ")

   **You have successfully completed the Lab**

## Summary

You should now have a introductory understanding of the basics of agentic applications in Oracle's AI Agent Studio!

## Acknowledgements
* **Author** - [](var:author)
* **Contributors** - [](var:contributors)
* **Last Updated By/Date** - [](var:last_updated)