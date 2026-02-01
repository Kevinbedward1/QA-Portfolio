# Session 1 - Contact Form Validation Exploration

Tester: Kevin Bedward

Application: Shady Meadows B&B

Date: December 22, 2025

Duration: 60 minutes

Charter: Explore Contact Form Validation

Test Environment: Microsoft Edge, Windows 11 Home, Lenovo 7i

Build/URL: [Restful-booker-platform demo](https://automationintesting.online/#contact)

1. **Charter**

Explore how the contact form handles valid and invalid inputs, including required fields, formatting rules, and error messaging.

1. **Areas Covered**

Name field

Email field

Phone field

Subject field

Message textarea

“Submit” button behavior

Success & error messages

1. **Test Notes**

**Tried**: Tried submitting the form blank - 

**Observed**: error message displayed for all fields. 

**Noticed**: It responded as expected, as the user cannot proceed.

**Question:** No questions to ask.

**Tried:** Entered 9895106 into the name field and clicked Submit 

**Observed:** Accepted as valid. The name field doesn’t restrict numeric-only input. **Noticed/Risk**: Users can enter invalid names, compromising data integrity. Users will enter information into the system, causing inefficiencies in the hotel’s operation. 

**Question:** Should the Name field restrict input to alphabetic characters, or is numeric input allowed?

**Tried:** Entered [kbedward.com](http://kbedward.com) into the email address field - **Observed**: received an error message: “must be a well-formed email address”. 

**Noticed/Risk:** It doesn’t indicate what is a well-formed email address. Risk that users may not know what a valid email address looks like. 

**Question:** Should the error message include an example (e.g. name@hotmail.com)?

**Tried:** Email was left blank and clicked Submit-

**Observed:**  error message received: “Email may not be blank”. It correctly responds that input wasn’t given. 

**Noticed:** No risk  -User cannot proceed. 

**Question**: No questions to ask.

**Tried:** Entered 256 in Phone field 

**Observed:**  error message received: “Phone must be between 11 and 21 characters”. 

**Noticed/Risk:** The error message is length-based only. It doesn’t state whether it should contain all numbers or if separators are allowed. Risk that users may not know what a valid phone number looks like. 

**Question:** Is the phone field expected to include country code, or strictly digits? That is dashes or spaces.

**Tried:** Entered 989999 in the Subject field and selected Submit.

 **Observed:**  accepted as valid. It cannot be left blank, but users aren’t restricted to what they can enter in the subject field. 

**Noticed:** Users can enter a subject that doesn’t have anything to do with the Hotel which reduces the usefulness of submissions. **Question:** Is it intentional for the Subject field to be opened without any restrictions, or should it have a dropdown menu with predefined options? 

**Tried:** Entered 522555552jjjjjjjjjjjjjjjj in the message field and selected Submit.

 **Observed:**  accepted as valid. 

**Noticed:** Users can enter information that doesn’t apply to the hotel’s processes, leading to unnecessary and low-quality submissions. 

**Question**: Should the field have restrictions or be an open form? 

**Tried:** Hovered and clicked submit.

 **Observed:**  it changed colour when the mouse was hovered over and again when clicked.  It shows the user that it is functional and clickable. 

**Noticed:** Users will be aware that to proceed, they will have to  click the button. 

Questions: No questions to ask.