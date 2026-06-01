# Putting it all together - Updating the workflow with the new custom agent

## Introduction

Now that you've built a new custom agent in the last lab, we will add the agent to our copy of the **Quote to Purchase Requisition Chat Assistant** template.
Finally we'll test the completed workflow to understand what debugging capabilities are provided during the development process.

Estimated Time: 15 minutes

### Objectives

How to add a node to a workflow and update an existing node.

Become familiar with the debugging tools provided during the development process.

### Usage Notes

   [](include:initial_hints)

## Task 1: Download Excel File
1. Download the sample quotation excel file **[HERE](files/quotation_sample.xlsx?download=1)**

Before we run the workflow, let’s prepare a purchase order PDF file needed to execute this agent.<br/>
Download the quotation **sample.xlsx** shared with this exercise.<br/>
Modify the Quotation Number value to replace **RITI** with your initials and save it as a PDF.<br/>
E.g., If your name is: **“Sheldon Cooper”**, quotation number will be: **SHCO_QUOTE6_260127**.

Save the excel file as a **PDF**.

   ![Sample Invoice](images/invoice.png " ")

## Task 2: Add our Custom Agent to the workflow

1. First we will open our workflow for editing.

   Click on **Agent Teams** tab.<br/>
2. Select the **Draft** button.<br/>
3. Enter ***YOUR INITIAL CODE*** in the search box.<br/>
4. Select the pencil icon to edit your workflow:

   ![Open Agent Team](images/open_agent_agent_team.png " ")

5. Next we will add our custom agent to the workflow.<br/><br/>
   Navagate  to the **Summarize the Requisition** LLM step. We will be adding our agent above this step.
   ![Naviagate to the LLM Step](images/step_to_edit.png " ")

6. Click on the **plus sign** just above the step to add a new step to the workflow.
   ![Add the new step](images/add_the_step_plus.png " ")

   Click on **AI** then **Agent** in the menu.
   ![Naviagate Menu](images/add_node_1.png " ")</br>

   Provide the following information in the dialog box.</br></br>
   **Important!**  Make sure to use **SupplierInquiryRestCall** as the name of the step.  This will match the text in the updated prompt in the LLM step.</br></br>
   Provide the rest of the information.</br>
   Search for the agent you created in the previous lab and select it.
   ![Menu Options](images/SupplierInquiry3.png " ")

   Now we will add the input variable. Click on the **pencil** icon to open up the menu.</br>

   ![Add Supervisor Agent](images/SupplierInquiryPencil.png =70%x*)
   Click on the **plus down arrow** to open up the menu.</br>
   From **Context** select **Variables** then **purchaseReqPayload**</br>
   ![Add Supervisor Agent](images/SupplierInquiryVariable.png =70%x*)
   This variable contains the information collected from the purchase order.</br>

      ![Navigate to variables](images/SupplierInquiryApply.png " ")
   Click on **Apply** when finished.
   Verify that you have the correct name for the step, the correct agent and the correct variable.  Click **Create** when done.
      ![Save the step configuration](images/SupplierInquiry4.png " ")
## Task 3: Updating the LLM Step

1. Navigate to the **Summarize the Requisition*** step.  Click on the lower right hand corner to open the menu.  Click on **Edit**.<br/>

   ![Update the prompt](images/update_the_prompt.png " ")


   Click **Copy** in the box below to copy the new prompt.
   ```txt
   <copy>
   You will have the data of requisition along with lines information in {{$context.$nodes.EXTRACT_REQUISITION_ATTRIBUTES_FROM_SUPPLIER_QUOTATION.$output}} . Using this information, output: The quote is from [[Supplier name]], with [[Number of lines]] lines and a total of $[[Total Requisition Amount]].
   I checked the supplier inventory.  {{$context.$nodes.SUPPLIERINQUIRYRESTCALL.$output}}.  Do you want to proceed to create the requisition?  If the supplier name is not present, use the file name.  Replace all bracketed placeholders with actual values. Do not include any extra commentary or explanation.
   Present the output in language {{$context.$variables.sessionLanguage}}.
   </copy>
    ```

2. Update the existing prompt.</br> Delete the old prompt and copy this new prompt and paste it into the text field.<br/>
   You  will notice in the red dialog that the output from our new node's output has been included in the new prompt. **{{$context.$nodes.SUPPLIERINQUIRYRESTCALL.$output}}**
   ![Summarize Step Select](images/update_prompt2.png " ")



   Click **Update** when complete.

   Click on Save and Close button saving your copy of the Purchase Requisition Chat Assistant.
   ![Summarize Step Select](images/save_and_close.png " ")


   **Congratulations!**  You have successfully completed Lab 3.

## Summary
   You now have an understanding of how to extend a pre-defined workflow template.<br/>

## Acknowledgements
* **Author** - [](var:author)
* **Contributors** - [](var:contributors)
* **Last Updated By/Date** - [](var:last_updated)