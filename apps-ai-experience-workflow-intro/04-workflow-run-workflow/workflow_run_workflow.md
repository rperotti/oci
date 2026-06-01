# See the Workflow in Action

## Introduction

Now that we have a completed workflow agent; you will run the agent, examine the output and get an introduction to the debugging tool in AI Agent Studio.

Estimated Time: 10 minutes

### Objectives

Understand how to run a workflow in the debugger.</br>
Examine the debugger output and how to drill into a step for more details.


## Task 1: Open the workflow & Run
1. Let's re-open workflow.

   Click on **Agent Teams** tab.<br/>
   Select the **Draft** button.<br/>
   Enter ***YOUR INITIAL CODE*** in the search box.<br/>
   Select the pencil icon to edit your agent team:

   ![Open Agent Team](images/draftmode2.png " ")

2. We will now run the agent in the debugger.  Click on the run button to get things started.</br></br>
   ![Run the agent in the debugger](images/start_debug.png " ")</br>

3. Upload the quotation</br>Upload the .PDF file we created in the previous lab.  Click on the **paperclip** icon to upload the file.</br>Once uploaded, type **create** in the input and press the **up arrow**.

   ![Upload the Quotation](images/ready_to_run.png " ")</br>
   As the workflow is executing, it will call our **SupplierInquiryRestCall** step that invoked the REST tool.  The tool will take the information passed in the variable we set which contains the parsed output of our requisition as input to the REST call.</br></br>
      ![Run the agent in the debugger](images/rest_call.png " ")</br>

4. Create the Requisition</br>
   You can see in the **Summarize the Requisition** step the prompt we updated is executed.  The output value from our custom agent step has been expanded to include the output from the REST call.</br></br>Notice the Approve or Reject buttons.  This is introduced by the **Get Feedback** step which required a human-in-the-loop approval to continue.</br>
   Click on **Approve** to continue.</br></br>
   ![Run the agent in the debugger](images/ready_to_create.png " ")</br>

   The workflow creates the requisition and returns a success message.  Included in the message is a deep link that you can click on and see your requisition that was created.</br>
      ![Deep link](images/success.png " ")</br>

5.Examine the  new  requisition.  **Right click** on the hyper-link to open the requisition in a new browser tab.
   ![New Requisition](images/requisition_complete.png " ")</br>

   **Congratulations!**  You have successfully created and tested your updated workflow!</br>
   **You have successfully completed the Lab!**
## Summary
   You now have an understanding of how to:</br></br>
   Copy a out-of-box template.</br>
   Create a new custom agent that uses REST tool.</br>
   Extend a pre-defined workflow template with a new step & modified prompt.</br>
   Understand how to navigate in AI Agent Studio to accomplish the above tasks <br/>

## Acknowledgements
* **Author** - [](var:author)
* **Contributors** - [](var:contributors)
* **Last Updated By/Date** - [](var:last_updated)