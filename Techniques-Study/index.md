# Techniques
## Tactic1 - [Reconnaissance](https://attack.mitre.org/tactics/TA0043)


<table>
<thead>
  <tr>
    <th>number</th>
    <th>Technique</th>
    <th>Sub-Techqniue</th>
    <th>Detection</th>
    <th>How to do</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>1</td>
    <td rowspan="2"><a href="https://attack.mitre.org/techniques/T1595" target="_blank" rel="noopener noreferrer">Active Scanning</a></td>
    <td><a href="https://attack.mitre.org/techniques/T1595/001" target="_blank" rel="noopener noreferrer">Scanning IP Blocks</a></td>
    <td>single source multiple dests</td>
    <td>nmap, netdiscover or other tools</td>
  </tr>
  <tr>
    <td>2</td>
    <td><a href="https://attack.mitre.org/techniques/T1595/002" target="_blank" rel="noopener noreferrer">Vulnerability Scanning</a></td>
    <td>malicious user-agents</td>
    <td>openvas, nessus, nmap, acunetix, ...</td>
  </tr>
  <tr>
    <td>3</td>
    <td rowspan="4"><a href="https://attack.mitre.org/techniques/T1592" target="_blank" rel="noopener noreferrer">Gather Victim Host Information</a></td>
    <td><a href="https://attack.mitre.org/techniques/T1592/001" target="_blank" rel="noopener noreferrer">Hardware</a></td>
    <td>Not possible</td>
    <td>active direct scan or phishing</td>
  </tr>
  <tr>
    <td>4</td>
    <td><a href="https://attack.mitre.org/techniques/T1592/002" target="_blank" rel="noopener noreferrer">Software</a></td>
    <td>Not possible</td>
    <td>active direct scan or phishing</td>
  </tr>
  <tr>
    <td>5</td>
    <td><a href="https://attack.mitre.org/techniques/T1592/003" target="_blank" rel="noopener noreferrer">Firmware</a></td>
    <td>Not possible</td>
    <td>active direct scan or phishing</td>
  </tr>
  <tr>
    <td>6</td>
    <td><a href="https://attack.mitre.org/techniques/T1592/004" target="_blank" rel="noopener noreferrer">Client Configurations</a></td>
    <td>Not possible</td>
    <td>active direct scan or phishing</td>
  </tr>
  <tr>
    <td>7</td>
    <td rowspan="3"><a href="https://attack.mitre.org/techniques/T1589" target="_blank" rel="noopener noreferrer">Gather Victim Identity Information</a></td>
    <td><a href="https://attack.mitre.org/techniques/T1589/001" target="_blank" rel="noopener noreferrer">Credentials</a></td>
    <td>Not possible</td>
    <td>Leaked DBs, phishing, compromise sites, keyloggers, ...</td>
  </tr>
  <tr>
    <td>8</td>
    <td><a href="https://attack.mitre.org/techniques/T1589/002" target="_blank" rel="noopener noreferrer">Email Addresses</a></td>
    <td>Not Possible</td>
    <td>OSINT, Leaked DBs, Social Medias</td>
  </tr>
  <tr>
    <td>9</td>
    <td><a href="https://attack.mitre.org/techniques/T1589/003" target="_blank" rel="noopener noreferrer">Employee Names</a></td>
    <td>Not Possible</td>
    <td>OSINT, Leaked DBs, Social Medias</td>
  </tr>
  <tr>
    <td>10</td>
    <td rowspan="6"><a href="https://attack.mitre.org/techniques/T1590" target="_blank" rel="noopener noreferrer">Gather Victim Network Information</a></td>
    <td><a href="https://attack.mitre.org/techniques/T1590/001" target="_blank" rel="noopener noreferrer">Domain Properties</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>11</td>
    <td><a href="https://attack.mitre.org/techniques/T1590/002" target="_blank" rel="noopener noreferrer">DNS</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>12</td>
    <td><a href="https://attack.mitre.org/techniques/T1590/003" target="_blank" rel="noopener noreferrer">Network Trust Dependencies</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>13</td>
    <td><a href="https://attack.mitre.org/techniques/T1590/004" target="_blank" rel="noopener noreferrer">Network Topology</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>14</td>
    <td><a href="https://attack.mitre.org/techniques/T1590/005" target="_blank" rel="noopener noreferrer">IP Addresses</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>15</td>
    <td><a href="https://attack.mitre.org/techniques/T1590/006" target="_blank" rel="noopener noreferrer">Network Security Appliances</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>16</td>
    <td rowspan="4"><a href="https://attack.mitre.org/techniques/T1591" target="_blank" rel="noopener noreferrer">Gather Victim Org Information</a></td>
    <td><a href="https://attack.mitre.org/techniques/T1591/002" target="_blank" rel="noopener noreferrer">Business Relationships</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>17</td>
    <td><a href="https://attack.mitre.org/techniques/T1591/001" target="_blank" rel="noopener noreferrer">Determine Physical Locations</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>18</td>
    <td><a href="https://attack.mitre.org/techniques/T1591/003" target="_blank" rel="noopener noreferrer">Identify Business Tempo</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>19</td>
    <td><a href="https://attack.mitre.org/techniques/T1591/004" target="_blank" rel="noopener noreferrer">Identify Roles</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>20</td>
    <td rowspan="3"><a href="https://attack.mitre.org/techniques/T1598" target="_blank" rel="noopener noreferrer">Phishing for Information</a></td>
    <td><a href="https://attack.mitre.org/techniques/T1598/001" target="_blank" rel="noopener noreferrer">Spearphishing Service</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>21</td>
    <td><a href="https://attack.mitre.org/techniques/T1598/002" target="_blank" rel="noopener noreferrer">Spearphishing Attachment</a></td>
    <td>Check emails / attachments</td>
    <td></td>
  </tr>
  <tr>
    <td>22</td>
    <td><a href="https://attack.mitre.org/techniques/T1598/003" target="_blank" rel="noopener noreferrer">Spearphishing Link</a></td>
    <td>Check emails / links</td>
    <td></td>
  </tr>
  <tr>
    <td>23</td>
    <td rowspan="2"><a href="https://attack.mitre.org/techniques/T1597" target="_blank" rel="noopener noreferrer">Search Closed Sources</a></td>
    <td><a href="https://attack.mitre.org/techniques/T1597/001" target="_blank" rel="noopener noreferrer">Threat Intel Vendors</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>24</td>
    <td><a href="https://attack.mitre.org/techniques/T1597/002" target="_blank" rel="noopener noreferrer">Purchase Technical Data</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>25</td>
    <td rowspan="5"><a href="https://attack.mitre.org/techniques/T1596" target="_blank" rel="noopener noreferrer">Search Open Technical Databases</a></td>
    <td><a href="https://attack.mitre.org/techniques/T1596/002" target="_blank" rel="noopener noreferrer">WHOIS</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>26</td>
    <td><a href="https://attack.mitre.org/techniques/T1596/001" target="_blank" rel="noopener noreferrer">DNS/Passive DNS</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>27</td>
    <td><a href="https://attack.mitre.org/techniques/T1596/003" target="_blank" rel="noopener noreferrer">Digital Certificates</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>28</td>
    <td><a href="https://attack.mitre.org/techniques/T1596/004" target="_blank" rel="noopener noreferrer">CDNs</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>29</td>
    <td><a href="https://attack.mitre.org/techniques/T1596/005" target="_blank" rel="noopener noreferrer">Scan Databases</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>30</td>
    <td rowspan="2"><a href="https://attack.mitre.org/techniques/T1593" target="_blank" rel="noopener noreferrer">Search Open Websites/Domains</a></td>
    <td><a href="https://attack.mitre.org/techniques/T1593/001" target="_blank" rel="noopener noreferrer">Social Media</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>31</td>
    <td><a href="https://attack.mitre.org/techniques/T1593/002" target="_blank" rel="noopener noreferrer">Search Engines</a></td>
    <td>Not Possible</td>
    <td></td>
  </tr>
  <tr>
    <td>32</td>
    <td><a href="https://attack.mitre.org/techniques/T1594" target="_blank" rel="noopener noreferrer">Search Victim-Owned Websites</a></td>
    <td>-</td>
    <td>Not Possible</td>
    <td></td>
  </tr>
</tbody>
</table>