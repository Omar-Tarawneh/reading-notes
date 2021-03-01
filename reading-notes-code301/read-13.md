# Read-12, 28 Feb 2021, Code 301

## Update & Delete

![request](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data/client-server.png)

sending form data is easy, but securing an application can be tricky. Just remember  a front-end developer is not the one who should define the security model of the data. It's possible to perform  client-side form validation, but the server can't trust this validation because it has no way to truly know what has really happened on the client-side.

**The action attribute**

 The action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL. If this attribute isn’t provided, the data will be sent to the URL of the page containing the form — the current page.


**The method attribute**
The  `method`  attribute specifies how to send form-data (the form-data is sent to the page specified in the  `action`  attribute).

The form-data can be sent as URL variables (with  `method="get"`) or as HTTP post transaction (with  `method="post"`).



- HTML forms [1](https://htmlreference.io/forms/)
- Styling forms [2](https://www.youtube.com/watch?v=HiHHvTcHiEk&list=PL4cUxeGkcC9g5_p_BVUGWykHfqx6bb7qK&index=1)

[GitHubPage-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code301/read-13)