

## Soho ReceiptPro
- A phone app that enables employees to take photos of their receipts for their expenses and automatically submit it to data source
- The app is powered by Microsoft Power Apps, Power Automate, Buildship, Airtable and Open AI.
- The app uses GPT vision to "read" the receipt and extract all details required, thus saving employees time

![image](https://github.com/user-attachments/assets/6a53a402-e997-48ea-ae3d-5b6f6d3a7fbd)


## ReceiptPro Demo

https://drive.google.com/file/d/1zo5MVRVaqjfIIWU-CHGeu5ZUQnuNXL99/view?usp=drive_link


## ReceiptPro Workflow


## Step 1: 
The first thing that happens is when a user opens their phone and submits the receipt.
So they take a photo of the receipt, upload it to the application, and click submit.
The next thing that happens is we have PowerApps saves the picture of a receipt to an Azure Data
storage bucket.

![image](https://github.com/user-attachments/assets/a62b90d7-ad0f-4f4a-a1ac-d93dd9278b8e)

## Step 2:
The next thing that will happen is once the user clicks submit, it will call a Power automate workflow,
which will then call a Buildship workflow as well.


![image](https://github.com/user-attachments/assets/b6007a01-5f15-4b43-983d-40f0179c68bb)

## Step 3:
Next, we call open AI with the photo of the receipt that was saved in Azure Data Storage.
OpenAI will take that photo from Azure Data Storage crunch it and return the values
that we need to populate the second page, which is the receipt date, the store name from the
receipt, the expense type, and the expense amount.

![image](https://github.com/user-attachments/assets/851d7bf2-a011-4ea8-b3f7-5f6bb53ee906)

## Step 4:
The next thing that the user will do is make any adjustments that they need to make and then click
submit to finalize their submission.
What happens after that is the information then goes to Power Automate first and then BuildShip, which then gets saved into a database within
Airtable.


![image](https://github.com/user-attachments/assets/999709cc-7c26-409b-bf2a-ad776dea36bc)

## BuildShip Flow

https://drive.google.com/file/d/1oFwyccJaBhGiiiDjnLp-HACImWmLCSZ1/view?usp=drive_link

![image](https://github.com/user-attachments/assets/72b6d047-e07e-4e87-9eda-7a0a243186ec)


![image](https://github.com/user-attachments/assets/4d864813-1211-4f56-9b8c-dd38db46d9d7)


## Power Automate Flows

![image](https://github.com/user-attachments/assets/d8eced5f-3863-4b61-a0ab-752c8938a512)


![image](https://github.com/user-attachments/assets/9534312d-417c-4485-86aa-53f82e529bd9)


![image](https://github.com/user-attachments/assets/d71f3ec4-e422-4793-b29c-5a48a16a44d4)


![image](https://github.com/user-attachments/assets/82fec5c7-4f9f-464b-bf23-a98de7542ce3)


![image](https://github.com/user-attachments/assets/70327ee6-6ba6-4a5f-88e7-437a397bb715)


![image](https://github.com/user-attachments/assets/c8be15c3-475a-4c43-a68e-4e163803566a)





## AirTable

![image](https://github.com/user-attachments/assets/ed25d244-a827-4a44-a314-bb82c694d612)












