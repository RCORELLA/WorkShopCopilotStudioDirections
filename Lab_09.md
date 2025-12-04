# Getting Started with Microsoft Copilot Studio

## Prerequisites
- Microsoft account with appropriate licenses
- Access to Copilot Studio (https://copilotstudio.microsoft.com)
- Admin or maker permissions in your environment

## Step 1: Access the agent

## Step 2: Create a new Tool

<img width="753" height="475" alt="image" src="https://github.com/user-attachments/assets/1f3b3c82-624c-4b3d-8f90-fbe9971dd34b" />

## Step 3: Create a Prompt

<img width="1456" height="590" alt="image" src="https://github.com/user-attachments/assets/154d0941-8742-4992-8145-29edbceacb63" />

## Step 4: Create the instructions

```
Extract invoice details, including vendor information, totals, and line items, from all pages of the invoice, ensuring that all relevant information is captured, even if it spans multiple pages. Identify and extract data from tables, including those containing checkboxes.
If a checkbox is unchecked, return "Not checked"; otherwise, extract the information.
Respond only with the results in JSON format.
The JSON object should include the following fields:  'PurchaseOrder', 'InvoiceId', 'InvoiceDate', 'DueDate', 'VendorName', 'VendorAddress', 'VendorAddressRecipient',  'SubTotal', 'TotalDiscount', 'TotalTax', 'InvoiceTotal', 'AmountDue', 'PreviousUnpaidBalance', 'RemittanceAddress', 'RemittanceAddressRecipient', 'ServiceAddress', 'ServiceAddressRecipient', 'ServiceStartDate', 'ServiceEndDate', 'VendorTaxId', 'CustomerTaxId', 'PaymentTerm', 'KVKNumber', 'PaymentDetails', 'PaymentDetails(IBAN)', 'PaymentDetails(SWIFT)', 'PaymentDetails(BankAccountNumber)', 'PaymentDetails(BPayBillerCode)', 'PaymentDetails(BPayReference)', 'TaxDetails', 'TaxDetails(Amount)', 'TaxDetails(Rate)', 'PaidInFourInstallements', 'PaidInFourInstallements(Amount)', 'PaidInFourInstallements(DueDate)', 'Items', 'Items(Amount)', 'Items(Date)', 'Items(Description)', 'Items(Quantity)', 'Items(ProductCode)', 'Items(Tax)', 'Items(TaxRate)', 'Items(Unit)', and 'Items(UnitPrice)'.

Example:
{
	"CustomerName": "029 PEUGEOT",
	"InvoiceId": "N B 455 009 98",
	"InvoiceDate": "15/06/18",
	"VendorName": "Adventure Works Cycles",
	"VendorAddress": "National Harbor, Marketing and Business division, Customer Service, Tel: 45 35 15 55 – Fax: 45 85 16 15",
	"Items": [
		{
			"Description": "TAX I SPS",
			"Quantity": 1,
			"UnitPrice": "10000",
			"Amount": "10000,00",
			"Stock": "Not checked"
		},
		{
			"Description": "Ship monitoring",
			"Quantity": "18358",
			"UnitPrice": "0,239",
			"Amount": "101873,00",
			"Stock": "Checked"
		}
	],
	"SubTotal": "894889,00",
	"TotalTax": "133184,00",
	"InvoiceTotal": "988073,00",
	"AmountDue": "988073,00"
}
Ignore blank fields from the response. Ensure the data is accurately parsed and compiled from each page of the document.

```
## Step 5: Define an input

<img width="863" height="403" alt="image" src="https://github.com/user-attachments/assets/c0099243-d5a7-4633-9a82-343e3d39b512" />

## Step 6: Test the prompt

<img width="1607" height="688" alt="image" src="https://github.com/user-attachments/assets/1b8cc0d0-45aa-4ce6-bd98-a5ef2f49298a" />


