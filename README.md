<svg width="440" height="210" viewBox="0 0 440 210" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      .bubble-text {
        font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
        font-size: 15px;
        line-height: 1.35;
        color: #1c1c1e;
        margin: 0;
      }
      .bubble-box {
        background: #e9e9eb;
        border-radius: 18px;
        padding: 10px 14px;
        display: inline-block;
        box-sizing: border-box;
      }
      .dot {
        fill: #8e8e93;
      }
    </style>
  </defs>

  <!-- ROW 1: "Hi, I'm Dalton" -->
  <g>
    <!-- typing dots -->
    <g>
      <animate attributeName="opacity" values="1;1;0;0" keyTimes="0;0.0857;0.0857;1" dur="14s" repeatCount="indefinite"/>
      <rect x="0" y="10" width="60" height="36" rx="18" fill="#e9e9eb"/>
      <circle class="dot" cx="18" cy="28" r="4">
        <animate attributeName="cy" values="28;22;28" dur="0.9s" begin="0s" repeatCount="indefinite"/>
      </circle>
      <circle class="dot" cx="30" cy="28" r="4">
        <animate attributeName="cy" values="28;22;28" dur="0.9s" begin="0.15s" repeatCount="indefinite"/>
      </circle>
      <circle class="dot" cx="42" cy="28" r="4">
        <animate attributeName="cy" values="28;22;28" dur="0.9s" begin="0.3s" repeatCount="indefinite"/>
      </circle>
    </g>

    <!-- bubble text -->
    <g>
      <animate attributeName="opacity" values="0;0;1;1" keyTimes="0;0.0857;0.0857;1" dur="14s" repeatCount="indefinite"/>
      <foreignObject x="0" y="6" width="260" height="44">
        <div xmlns="http://www.w3.org/1999/xhtml" class="bubble-box">
          <p class="bubble-text">Hi, I'm Dalton</p>
        </div>
      </foreignObject>
    </g>
  </g>

  <!-- ROW 2: "I'm an Intelligence analyst researching emerging cyber threats." -->
  <g>
    <!-- typing dots -->
    <g>
      <animate attributeName="opacity" values="0;0;1;1;0;0" keyTimes="0;0.2857;0.2857;0.371;0.371;1" dur="14s" repeatCount="indefinite"/>
      <rect x="0" y="66" width="60" height="36" rx="18" fill="#e9e9eb"/>
      <circle class="dot" cx="18" cy="84" r="4">
        <animate attributeName="cy" values="84;78;84" dur="0.9s" begin="0s" repeatCount="indefinite"/>
      </circle>
      <circle class="dot" cx="30" cy="84" r="4">
        <animate attributeName="cy" values="84;78;84" dur="0.9s" begin="0.15s" repeatCount="indefinite"/>
      </circle>
      <circle class="dot" cx="42" cy="84" r="4">
        <animate attributeName="cy" values="84;78;84" dur="0.9s" begin="0.3s" repeatCount="indefinite"/>
      </circle>
    </g>

    <!-- bubble text -->
    <g>
      <animate attributeName="opacity" values="0;0;1;1" keyTimes="0;0.371;0.371;1" dur="14s" repeatCount="indefinite"/>
      <foreignObject x="0" y="62" width="360" height="64">
        <div xmlns="http://www.w3.org/1999/xhtml" class="bubble-box">
          <p class="bubble-text">I'm an Intelligence analyst, researching emerging cyber threats.</p>
        </div>
      </foreignObject>
    </g>
  </g>

  <!-- ROW 3: "Welcome to my page" -->
  <g>
    <!-- typing dots -->
    <g>
      <animate attributeName="opacity" values="0;0;1;1;0;0" keyTimes="0;0.643;0.643;0.729;0.729;1" dur="14s" repeatCount="indefinite"/>
      <rect x="0" y="150" width="60" height="36" rx="18" fill="#e9e9eb"/>
      <circle class="dot" cx="18" cy="168" r="4">
        <animate attributeName="cy" values="168;162;168" dur="0.9s" begin="0s" repeatCount="indefinite"/>
      </circle>
      <circle class="dot" cx="30" cy="168" r="4">
        <animate attributeName="cy" values="168;162;168" dur="0.9s" begin="0.15s" repeatCount="indefinite"/>
      </circle>
      <circle class="dot" cx="42" cy="168" r="4">
        <animate attributeName="cy" values="168;162;168" dur="0.9s" begin="0.3s" repeatCount="indefinite"/>
      </circle>
    </g>

    <!-- bubble text -->
    <g>
      <animate attributeName="opacity" values="0;0;1;1" keyTimes="0;0.729;0.729;1" dur="14s" repeatCount="indefinite"/>
      <foreignObject x="0" y="146" width="260" height="44">
        <div xmlns="http://www.w3.org/1999/xhtml" class="bubble-box">
          <p class="bubble-text">Welcome to my page.</p>
        </div>
      </foreignObject>
    </g>
  </g>
</svg>

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
