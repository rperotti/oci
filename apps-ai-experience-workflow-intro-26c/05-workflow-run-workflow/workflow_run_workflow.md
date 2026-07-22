# See the Workflow in Action

## Introduction

Now that we have a completed workflow agent; you will run the agent, examine the output and get an introduction to the debugging tool in AI Agent Studio.

Estimated Time: 10 minutes

### Objectives

Understand how to run a workflow in the debugger.</br>
Examine the debugger output and how to drill into a step for more details.


## Task 1: Run the workflow

   ![Open Agent Team](images/run_debug.png " ")
   1. We will now run the agent in the debugger.  Click on the **debug** button to get things started.</br></br>
   ![Open Agent Team](images/upload_document.png " ")
   2. Upload the .PDF file we downloaded in Lab1.  Click on the **paperclip** icon to upload the file.</br>.
   ![Open Agent Team](images/type_create.png " ")
   3. Once uploaded, type **create** and press return.
   ![Open Agent Team](images/debug_output.png " ")
   4. Scroll down to the REST node we added.  Click on the node to see the debug output.  You can see the data from the **purchaseRequisitionObject** that we leverage as input for the node.</br>
   You can also see the input to the REST call and the information the REST call returned with the inventory status.
   ![Get Feedback Node](images/get_feedback.png " ")
   5. The Get Feedback node is a human in the loop node.  The workflow prompts the user to continue before creating the requisition.</br>
   ![Approve to create the requisition](images/click_approve.png " ")
   6. Click Approve to create the requisition.
   ![Approve to create the requisition](images/output_from_workflow.png " ")
   6. When the workflow completes, you will see a hyper-link to the new requisition.
   **Click** on the hyper-link to see your newly created requisition.
   ![Open Agent Team](images/new_object.png " ")

   **Congratulations!**  You have successfully created and tested your workflow!</br>
   **You have successfully completed the Lab!**
## Summary
   You now have an understanding of how to:</br></br>
   Copy a existing workflow.</br>
   Create a new node that uses REST tool.</br>
   Update a existing LLM node to add our new functionallity to it.</br>
   Understand how to navigate in AI Agent Studio to accomplish the above tasks <br/>

## Acknowledgements
* **Author** - [](var:author)
* **Contributors** - [](var:contributors)
* **Last Updated By/Date** - [](var:last_updated)