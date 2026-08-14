# Exploring a pre-built workflow template

## Introduction

In this lab we will copy an existing workflow and do a walkthrough to get an understanding of the various nodes and functionality of the workflow as well as a brief introduction to the workflow editor.

Estimated Time: 10 minutes

### Objectives

Understand the structure of a workflow and agent tools in AI Agent Studio.

### Usage Notes

   [](include:initial_hints)

## Task 1: Login and navigate to the AI Agent Studio Landing Page

1. First you will log in and navigate to AI Agent Studio.

   Login to the lab environment using the credentials provided.  Navigate to the AI Agent Studio tile and click on it.</br>

2. Go to the **Tools** tab and Click on the tile for **AI Agent Studio**:
3. Click on the AI Agent Studio tile
   ![AI Agent Tile in Fusion](images/LoggedIn.png " ")

4. On the AI Agent Studio landing page we are going to click on **Workflows**.
   ![AI Agent Landing Pages](images/landing_page.png " ")

5. We are going to make a copy of a published workflow.  In the search window type **AIE MASTER** for the search string.  When you have located the **published** workflow, click on the **duplicate** button to copy the workflow.
    Make sure you click on **DUPLICATE**
   ![Search for the workflow](images/copy_template.png " ")

6. Make sure to use ***YOUR INITIAL CODE*** when naming the template.<br/>
   ![Duplicating the master workflow](images/unique_name.png " ")

7. Now that we have our own copy of the workflow we can explore some of the nodes and features.</br>
   ![Workflow copied](images/inside_the_workflow.png =60%x*)

## Task 2: Examine the Workflow

1. Examine the Workflow</br>
   Starting in 26C you now have a very powerful wizard or 'agentic brain' available in the workflow editor that can troubleshoot/explain and update workflows & resources just by asking it questions.  We are going to use this feature to explain the workflow and nodes in the workflow.</br></br>
    Click on the icon at the bottom of the page to get started.</br>
    ![Invoking the Agentic Brain](images/AI_Helper.png =60%x*)</br>


   Scroll down to the **Get User Session Information** node.
   Ask the wizard to explain this node - **"Tell me about the get user session information node"**</br>
   ![User Session Details](images/get_user_session.png =60%x*)

2. Examine The Get Intent Node</br>
   Scroll down to the **Get Intent** node.
      Ask the wizard to explain this node - **"Tell me about the Get Intent node"**</br>
   ![Agent Brain's provides details about this node ](images/explain_get_intent_node_2.png =60%x*)
   The Get Intent Node leverages a LLM to determine the intent of the user's input.  In this workflow it's specifically looking to see if the user want to create a requisition.</br>

   Click on the **Get Intent Node**.  You can see from the prompt, the users input is used by the LLM to identify what action was requested.</br>
   ![Details of the LLM Node](images/get_intent_details.png =70%x*)</br>
   This completes our examination of a few of the nodes in this workflow.



## Task 3: Download the Example Quotation File

1. Download the Example Quotation File

   This sample quote file will be used when we run our modified workflow.

   Download the sample quotation PDF file: **[CLICK HERE TO DOWNLOAD THE PDF QUOTE FILE](files/aie_quotation_sample.pdf?download=1)**</br>
   </br>**You have successfully completed Module 1!**

## Summary

You should now have a brief introductory understanding of some the tools and prompts used in this sample workflow.<br/>
In the next lab we will add an additional node to expand the capabilities of this workflow.

[Proceed to the next lab](#next)

## Acknowledgements
* **Author** - [](var:author)
* **Contributors** - [](var:contributors)
* **Last Updated By/Date** - [](var:last_updated)