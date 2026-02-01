<input type="text" id="nameInput" placeholder="Ievadi savu vārdu">
<button onclick="showGreeting()">Sveicināt</button>
<p id="message"></p>
function showGreeting() {
    let userName = document.getElementById("nameInput").value;
    let message = document.getElementById("message");

    if (userName === "") {
        message.style.color = "red";
        message.innerHTML = "Lūdzu, ievadi savu vārdu!";
    } else {
        message.style.color = "green";
        message.innerHTML = "Sveiks, " + userName + "! Prieks tevi redzēt!";
    }
}

