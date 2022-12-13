# UnobtrusiveContactFormUmbraco9and10
Unobtrusive Contact Form Umbraco 9  and 10  


1) In the master template add:

<script src="https://ajax.aspnetcdn.com/ajax/jQuery/jquery-3.6.0.js"></script>
<script src="https://ajax.aspnetcdn.com/ajax/jquery.validate/1.16.0/jquery.validate.min.js"></script>
<script src="https://ajax.aspnetcdn.com/ajax/jquery.validation.unobtrusive/3.2.6/jquery.validate.unobtrusive.min.js"></script>

2) Add the View Model, The Controler and the Contact Partial and the ContactMessageSentPartial

3) In the Contact form View add a Using to the Models and pass the Model in to the partial:

@using MyApp.Models;

@await Html.PartialAsync("_contactForm", new ContactFormViewModel())


ToDo:  ADD RECAPTCHA

1) Install via nuget AspNetCore.ReCaptcha
