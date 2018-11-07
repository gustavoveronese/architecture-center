---
title: Azure Example Scenario
description: Example Scenarios that solve specific business use cases
author: david-stanford
ms:date: 08/01/2018
layout: LandingPage
ms.topic: landing-page
---
# Azure Example Scenarios

Example scenarios walk through the process of solving specific architectural and business problems on Azure.  Each scenario is based on a real customer example and is intended to provide fast, easy to read guidance to help accelerate your own implementation.

Within each scenario you can find an architecture diagram, data flows, and details of all of the components.  You can also learn about alternatives technologies that may better fit your business need, rough pricing of the solution, and considerations when running the solution in production.  Many scenarios will also contain a method to easily deploy the solution in your own Azure account.

Jump to: [AI scenarios](#ai-scenarios) | [Application scenarios](#application-scenarios) | [Data scenarios](#data-scenarios) | [Infrastructure scenarios](#infrastructure-scenarios)


<style>
* {
  box-sizing: border-box;
}

#myInput {
  background-image: url('/css/searchicon.png');
  background-position: 10px 12px;
  background-repeat: no-repeat;
  width: 100%;
  font-size: 16px;
  padding: 12px 20px 12px 40px;
  border: 1px solid #ddd;
  margin-bottom: 12px;
}

#myUL {
  list-style-type: none;
  padding: 0;
  margin: 0;
}

#myUL li a {
  border: 1px solid #ddd;
  margin-top: -1px; /* Prevent double borders */
  background-color: #f6f6f6;
  padding: 12px;
  text-decoration: none;
  font-size: 18px;
  color: black;
  display: block
}

#myUL li a:hover:not(.header) {
  background-color: #eee;
}
</style>


<h2>My Phonebook</h2>

<input type="text" id="myInput" onkeyup="myFunction()" placeholder="Search for names.." title="Type in a name">

<ul id="myUL">
  <li><a href="#">Adele</a></li>
  <li><a href="#">Agnes</a></li>

  <li><a href="#">Billy</a></li>
  <li><a href="#">Bob</a></li>

  <li><a href="#">Calvin</a></li>
  <li><a href="#">Christina</a></li>
  <li><a href="#">Cindy</a></li>
</ul>

<script>
function myFunction() {
    var input, filter, ul, li, a, i;
    input = document.getElementById("myInput");
    filter = input.value.toUpperCase();
    ul = document.getElementById("myUL");
    li = ul.getElementsByTagName("li");
    for (i = 0; i < li.length; i++) {
        a = li[i].getElementsByTagName("a")[0];
        if (a.innerHTML.toUpperCase().indexOf(filter) > -1) {
            li[i].style.display = "";
        } else {
            li[i].style.display = "none";
        }
    }
}
</script>


<ul class="panelContent cardsL">
    <li>
        <div class="cardSize">
            <div class="cardPadding">
                <div class="card">
                    <div class="cardText">
                        <h3>New Scenarios</h3>
                        <a class="barLink" href="/azure/architecture/example-scenario/apps/decentralized-trust" data-linktype="absolute-path">Decentralized trust between banks on Azure</a>
                        <a class="barLink" href="/azure/architecture/example-scenario/infrastructure/wordpress" data-linktype="absolute-path">Highly scalable and secure WordPress website</a>
                        <a class="barLink" href="/azure/architecture/example-scenario/data/data-warehouse" data-linktype="absolute-path">Data warehousing & analytics for sales and marketing</a>
                    </div>
                </div>
            </div>
        </div>
    </li>
    <li>
        <div class="cardSize">
            <div class="cardPadding">
                <div class="card">
                    <div class="cardText">
                        <h3>Top Scenarios</h3>
                        <a class="barLink" href="/azure/architecture/example-scenario/ai/intelligent-apps-image-processing" data-linktype="absolute-path">Image classification for insurance claims</a>
                        <a class="barLink" href="/azure/architecture/example-scenario/apps/commerce-chatbot" data-linktype="absolute-path">Conversational chatbot for hotel reservations</a>
                        <a class="barLink" href="/azure/architecture/example-scenario/infrastructure/regulated-multitier-app" data-linktype="absolute-path">Secure Windows web application for regulated industries</a>
                    </div>
                </div>
            </div>
        </div>
    </li>
    <li>
        <div class="cardSize">
            <div class="cardPadding">
                <div class="card">
                    <div class="cardText">
                        <a href="https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRy0ZnoKOXdVBqaBz653YPElUNjlNMEpPMDNSSU1aWEIxMFNFNlY2T0E3NC4u" data-linktype="external">
                            <div class="cardSize cardsF">
                                <div class="cardPadding">
                                    <div class="card">
                                        <div class="cardImageOuter">
                                            <div class="cardImage">
                                                <img src="https://docs.microsoft.com/en-us/media/common/i_feedback.svg" alt="" data-linktype="external">
                                            </div>
                                        </div>
                                        <div class="cardText">
                                            <h3 class="x-hidden-focus">Submit your idea for a new scenario</h3>
                                            <p>Do you have a scenario that you'd like us to create?</p>
                                            <p>Would you like to build one yourself?</p>
                                            <p>Submit your idea here!</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </li>
</ul>

[!INCLUDE [notes](./articles.md)]