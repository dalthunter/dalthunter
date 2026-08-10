<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Apple Text Animation</title>

<style>
    * {
        box-sizing: border-box;
    }

    body {
        margin: 0;
        min-height: 100vh;
        display: flex;
        align-items: center;
        justify-content: center;
        background: #000;
        font-family: -apple-system, BlinkMacSystemFont, "SF Pro Display",
                     "SF Pro Text", Helvetica, Arial, sans-serif;
    }

    .phone {
        width: 390px;
        height: 844px;
        background: #f5f5f7;
        border-radius: 45px;
        overflow: hidden;
        box-shadow: 0 0 60px rgba(255,255,255,0.08);
        display: flex;
        flex-direction: column;
    }

    /* iPhone-style header */
    .header {
        height: 105px;
        padding-top: 48px;
        background: rgba(250,250,250,0.96);
        border-bottom: 1px solid #d8d8d8;
        display: flex;
        align-items: center;
        justify-content: center;
        position: relative;
    }

    .back {
        position: absolute;
        left: 20px;
        font-size: 27px;
        color: #007aff;
        font-weight: 300;
    }

    .contact {
        text-align: center;
    }

    .avatar {
        width: 31px;
        height: 31px;
        margin: 0 auto 2px;
        border-radius: 50%;
        background: #d1d1d6;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 15px;
        color: white;
    }

    .contact-name {
        font-size: 12px;
        font-weight: 500;
        color: #333;
    }

    .messages {
        flex: 1;
        padding: 20px 14px;
        display: flex;
        flex-direction: column;
        justify-content: flex-end;
        gap: 7px;
        overflow: hidden;
    }

    /* Incoming message */
    .message {
        align-self: flex-start;
        max-width: 78%;
        background: #e5e5ea;
        color: #000;
        padding: 9px 14px;
        border-radius: 19px;
        font-size: 17px;
        line-height: 1.25;
        opacity: 0;
        transform: translateY(10px);
        animation: messageIn 0.25s ease forwards;
    }

    /* Typing indicator */
    .typing {
        align-self: flex-start;
        background: #e5e5ea;
        width: 58px;
        height: 36px;
        border-radius: 19px;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 4px;
        opacity: 0;
        transform: translateY(10px);
    }

    .dot {
        width: 7px;
        height: 7px;
        border-radius: 50%;
        background: #777;
        animation: typing 1.2s infinite ease-in-out;
    }

    .dot:nth-child(2) {
        animation-delay: 0.15s;
    }

    .dot:nth-child(3) {
        animation-delay: 0.3s;
    }

    @keyframes typing {
        0%, 60%, 100% {
            transform: translateY(0);
            opacity: 0.45;
        }

        30% {
            transform: translateY(-4px);
            opacity: 1;
        }
    }

    @keyframes messageIn {
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }

    .show {
        opacity: 1;
        transform: translateY(0);
    }

    /* Replay button */
    .replay {
        position: absolute;
        bottom: 25px;
        right: 25px;
        border: none;
        background: #007aff;
        color: white;
        padding: 10px 17px;
        border-radius: 20px;
        font-size: 14px;
        cursor: pointer;
        font-family: inherit;
    }

    .replay:hover {
        background: #006ee6;
    }

</style>
</head>

<body>

<div class="phone">

    <div class="header">
        <div class="back">‹</div>

        <div class="contact">
            <div class="avatar">D</div>
            <div class="contact-name">Dalton</div>
        </div>
    </div>

    <div class="messages" id="messages"></div>

</div>

<button class="replay" onclick="startAnimation()">Replay</button>


<script>

const messages = [
    "Hi there 👋",
    "My name is Dalton.",
    "I'm an Intelligence Analyst researching emerging cyber threats."
    "Welcome to my page."
];

const messagesContainer = document.getElementById("messages");


function createTypingIndicator() {

    const typing = document.createElement("div");

    typing.className = "typing";

    typing.innerHTML = `
        <div class="dot"></div>
        <div class="dot"></div>
        <div class="dot"></div>
    `;

    messagesContainer.appendChild(typing);

    requestAnimationFrame(() => {
        typing.classList.add("show");
    });

    return typing;
}


function createMessage(text) {

    const message = document.createElement("div");

    message.className = "message";
    message.textContent = text;

    messagesContainer.appendChild(message);

    return message;
}


function wait(ms) {
    return new Promise(resolve => setTimeout(resolve, ms));
}


async function startAnimation() {

    messagesContainer.innerHTML = "";

    // First typing indicator
    let typing = createTypingIndicator();

    await wait(1800);

    // Remove typing indicator
    typing.remove();

    // First message
    createMessage(messages[0]);

    await wait(1000);

    // Second typing indicator
    typing = createTypingIndicator();

    await wait(1800);

    typing.remove();

    // Second message
    createMessage(messages[1]);

    await wait(1000);

    // Third typing indicator
    typing = createTypingIndicator();

    await wait(1800);

    typing.remove();

    // Third message
    createMessage(messages[2]);
}


// Start automatically
startAnimation();

</script>

</body>
</html>

## 👤 Threat Actor Profiles
**[The Gentlemen](https://dalthunter.github.io/intel-reports/gentlemen/)** ➜ Ransomware-as-a-Service (RaaS)

**[Scattered Spider](https://dalthunter.github.io/intel-reports/scattered-spider/)** ➜ Social Engineering & Identity Attacks

**[ShinyHunters](https://dalthunter.github.io/intel-reports/shinyhunters/)** ➜ Data Extortion & Cloud Intrusions

**[FIN7](https://dalthunter.github.io/intel-reports/fin7/)** ➜ Financial Cybercrime & Enterprise Intrusions

**[UNC6040](https://dalthunter.github.io/intel-reports/UNC6040/)** ➜ Cloud Identity & Voice Phishing (Vishing)

**[Lazarus Group](https://dalthunter.github.io/intel-reports/lazarus-group/)** ➜ Nation-State Cyber Operations & Financial Theft

**[Volt Typhoon](https://dalthunter.github.io/intel-reports/volt-typhoon/)** ➜ Critical Infrastructure & Living-off-the-Land

**[TraderTraitor](https://dalthunter.github.io/intel-reports/tradertraitor/)** ➜ Cryptocurrency Theft & Supply Chain Attacks

**[Luna Moth](https://dalthunter.github.io/intel-reports/luna-moth/)** ➜ Callback Phishing & Data Extortion
***
## 👤 Tactics, Techniques, and Procedures
<table>
<tr>
<td style="font-size: 1.2em;"><strong> Reconnaissance — <a href="https://attack.mitre.org/tactics/TA0043/">TA0043</a></strong></td>
<td style="font-size: 1.2em;">➜ Find information about the target.</td>
</tr>

<tr>
<td style="font-size: 1.2em;"><strong> Resource Development — <a href="https://attack.mitre.org/tactics/TA0042/">TA0042</a></strong></td>
<td style="font-size: 1.2em;">➜ Prepare infrastructure, malware, accounts, or credentials.</td>
</tr>

<tr>
<td style="font-size: 1.2em;"><strong> Initial Access — <a href="https://attack.mitre.org/tactics/TA0001/">TA0001</a></strong></td>
<td style="font-size: 1.2em;">➜ Get into the victim's system.</td>
</tr>

<tr>
<td style="font-size: 1.2em;"><strong> Execution — <a href="https://attack.mitre.org/tactics/TA0002/">TA0002</a></strong></td>
<td style="font-size: 1.2em;">➜ Run malicious code or commands.</td>
</tr>

<tr>
<td style="font-size: 1.2em;"><strong> Persistence — <a href="https://attack.mitre.org/tactics/TA0003/">TA0003</a></strong></td>
<td style="font-size: 1.2em;">➜ Stay in the system after gaining access.</td>
</tr>

<tr>
<td style="font-size: 1.2em;"><strong> Privilege Escalation — <a href="https://attack.mitre.org/tactics/TA0004/">TA0004</a></strong></td>
<td style="font-size: 1.2em;">➜ Gain higher-level permissions.</td>
</tr>

<tr>
<td style="font-size: 1.2em;"><strong> Defense Evasion — <a href="https://attack.mitre.org/tactics/TA0005/">TA0005</a></strong></td>
<td style="font-size: 1.2em;">➜ Hide activity and avoid detection.</td>
</tr>

<tr>
<td style="font-size: 1.2em;"><strong> Credential Access — <a href="https://attack.mitre.org/tactics/TA0006/">TA0006</a></strong></td>
<td style="font-size: 1.2em;">➜ Steal passwords, tokens, or other credentials.</td>
</tr>

<tr>
<td style="font-size: 1.2em;"><strong> Discovery — <a href="https://attack.mitre.org/tactics/TA0007/">TA0007</a></strong></td>
<td style="font-size: 1.2em;">➜ Find systems, users, networks, and valuable data.</td>
</tr>

<tr>
<td style="font-size: 1.2em;"><strong> Lateral Movement — <a href="https://attack.mitre.org/tactics/TA0008/">TA0008</a></strong></td>
<td style="font-size: 1.2em;">➜ Move from one compromised system to another.</td>
</tr>

<tr>
<td style="font-size: 1.2em;"><strong> Command and Control — <a href="https://attack.mitre.org/tactics/TA0011/">TA0011</a></strong></td>
<td style="font-size: 1.2em;">➜ Communicate with attacker-controlled infrastructure.</td>
</tr>

<tr>
<td style="font-size: 1.2em;"><strong> Collection — <a href="https://attack.mitre.org/tactics/TA0009/">TA0009</a></strong></td>
<td style="font-size: 1.2em;">➜ Gather valuable information from the victim.</td>
</tr>

<tr>
<td style="font-size: 1.2em;"><strong> Exfiltration — <a href="https://attack.mitre.org/tactics/TA0010/">TA0010</a></strong></td>
<td style="font-size: 1.2em;">➜ Move stolen data outside the victim's network.</td>
</tr>

<tr>
<td style="font-size: 1.2em;"><strong> Impact — <a href="https://attack.mitre.org/tactics/TA0040/">TA0040</a></strong></td>
<td style="font-size: 1.2em;">➜ Disrupt, destroy, encrypt, or expose systems and data.</td>
</tr>
</table>

<img width="383" height="514" alt="image" src="https://github.com/user-attachments/assets/68194ba4-27d6-4d09-9fd3-7e2b15d861c6" /> <img width="383" height="514" alt="image" src="https://github.com/user-attachments/assets/20c014c3-fa25-4804-a8f8-b14bcbb22a34" />

***
