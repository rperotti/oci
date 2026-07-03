# Exploring a pre-built workflow template

## Introduction

In this lab we will upload a exported workflow template, save it and get an walkthrough of the template to get aunderstanding of the various components and large language model (LLM) use.

Estimated Time: 15 minutes

### Objectives

Understand the structure of a pre-built workflow template and agent tools in AI Agent Studio.

### Usage Notes

   [](include:initial_hints)

## Task 1: Login and navigate to the AI Agent Studio Landing Page.

1. First you will log in and navigate to AI Agent Studio.

   Login to the lab environment using the credentials provided. Make sure to use your assigned user.  Navigate to the AI Agent Studio Tab and click on it.</br>

2. Go to the **Tools** tab and Click on the tile for **AI Agent Studio**:

   ![Application Home](images/image001.png " ")
3. Clicking on the Ai Agent Studio tab will take you to the AI Agent Studio landing page.  

Next we will move to the **Agent Teams** window. The Agent Teams tab is located at the bottom of the page.  
   ![Application Home](images/landing_page_agent_team.png =70%x*)
Click on Agent Teams at the bottom of the page.<br/>
   ![Application Home](images/agent_team_page_no_red_box.png =70%x*)
## Task 2: Download and Edit the Workflow JSON File
1. Download the sample workflow file: **[DOWNLOAD FILE - CLICK HERE](files/QUOTE_TO_PURCHASE_REQUISITION_CHAT_ASSISTANT_STARTER.json?download=1)**

2. Open the QUOTE_TO_PURCHASE_REQUISITION_CHAT_ASSISTANT_STARTER.json file with an editor, Notepad, Visual Studio, textpad, etc.  **DO NOT USE Microsoft Word!**

3. Scroll to the bottom of the file

   ![Move to the bottom of the text file](images/edit_in_text_pad.png " ")
4. On the line beginning with "WorkflowCode:" Replace **_STARTER** with a underbar and your initials in UPPERCASE <br/>
5. On the next line beginning with "Name":" Replace **STARTER** with your initials in **UPPERCASE** <br/>
   ![Replace the Name](images/edit_updated_with_new_names.png " ")

6. Once complete.  You will need to *SAVE AS* the end of the file name with your initials.

   ![Rename file with your initials](images/change_file_name.png " ")

   ![Caution](images/caution.png =50x*)  ***IMPORTANT!*** <br/>
   **Verify that you have make the two changes to the file with your initials**<br/>
   **Verify you have re-named the file with an underbar and your initials in UPPERCASE**.


## Task 3: Import the file into AI Agent Studio

1. On the Agent Teams page, click on the Import button.<br/>
   ![Import workflow file](images/import.png =70%x*)

2. Once you complete the import you will search for your imported workflow agent.<br/>Verify that the Draft button is selected then type in the initials you used to update the import file in the search box.<br/>Click on the pencil icon to open the workflow.
   ![Import the file](images/locate_agent.png " ")

   In the next task we will examine the agent.

   ![Examine the Agent](images/exmaine_the_agent.png " ")

   >![Check](images/check.png =90x*) ***STATUS CHECKPOINT*** <br/>
   > If you do not see your workflow, return to step 2

   **You have successfully completed Task 3!**

## Task 4: Examine the pre-built Quote to Purchase Requisition Chat Assistant template components

1. Let's take a closer look at the Get User Session Step

3. Click on the **Gear** button in the upper left hand corner of the screen.
- **LLM**: This Agent Team has the default LLM set.
- **Chat Experience**: It has enabled Enable File Upload in Chat Experience so that documents can be uploaded.
- **Variables**: It has four variable defined.

![Image alt text](images/DetailsDialog.png =50%x*)

4. Examine a node

Now let’s review one of the nodes of this agent. Open the **Get User Session Information** node to review its setup.

![Image alt text](images/EditSessionButton.png =50%x*)

Note that function **getUserSession** under business object **Self Detail** is set to be used in this node.
Optionally, you can navigate to the **Business Object** tab at the bottom of the page and query up this Business Object to see it’s setup in more detail.

![Image alt text](images/GetUserSessionDetail.png =50%x*)

5. Continue to examine a node

Scroll further down the page and note that the JSON specification has been entered. The results of the business object will
be returned in this format, and the use of the JSON specification means that the attributes can be referred to directly in
subsequent nodes.

![Image alt text](images/GetUserSessionMoreDetail.png =50%x*)

6. Examine Other Nodes

Feel free to review other types of nodes in this workflow When done, proceed to the next step where we will creating and adding a new agent to the workflow.

Click on **Save and Close** button saving your copy of the Purchase Requisition Chat Assistant:

   ![agent header save and close](images/save_and_close_after_explore.png " ")

   **You have successfully completed Module 1!**

   
## Summary

You should now have a introductory understanding of the tools and prompts provided by the pre-built Quote to Purchase Requisition Status Advisor workflow template.<br/>
In the next lab we will create a custom agent to expand the capabilities of this workflow.

[Proceed to the next lab](#next)

## Acknowledgements
* **Author** - [](var:author)
* **Contributors** - [](var:contributors)
* **Last Updated By/Date** - [](var:last_updated)