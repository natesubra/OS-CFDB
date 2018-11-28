# Finding Details 

### Finding Matrix
| Title  | VSR  |  CVSS  | Risk |
|:-:|:-:|:-:|:-:|
|  Stored XSS  |  4 |  5.1-7.5 | Medium-High  |

### Finding Service
| Service  |
|:-:|
| Internal Penetration Testing  |
| External Penetration Testing  |

### Finding NIST 800-53 Controls
| NIST  |
|:-:|
| SI-10  |
| RA-5   |
| CA-8   |
| PT-3   |
| AE-2   |
| CM-4   |

### Finding MITRE ATT&CK Corelation
| Name | Tactic | ID | Link |
|:-:|:-:|:-:|:-:|
| Exploitation for Client Execution | Execution | T1203 | https://attack.mitre.org/wiki/Technique/T1203 |

### Finding Refrences
| URL |
|:-:|
| https://nvd.nist.gov/download/800-53/800-53-controls.xml |
| https://www.owasp.org/index.php/Cross-site_Scripting_(XSS) |
| https://attack.mitre.org/wiki/Technique/T1203 |
| https://csrc.nist.gov/Glossary/?term=5519 |
# Technical Information

### Description 
A vulnerability that allows attackers to inject malicious code into an otherwise benign website. These scripts acquire the permissions of scripts generated by the target website and can therefore compromise the confidentiality and integrity of data transfers between the website and client. Websites are vulnerable if they display user supplied data from requests or forms without sanitizing the data so that it is not executable. Stored attacks are those where the injected script is permanently stored on the target servers, such as in a database, in a message forum, visitor log, comment field, etc. The victim then retrieves the malicious script from the server when it requests the stored information. Stored XSS is also sometimes referred to as Persistent or Type-I XSS.
### Impact
The impact  of an XSS attack is the same regardless of whether it is stored or reflected (or DOM Based). The difference is in how the payload arrives at the server. Do not be fooled into thinking that a “read only” or “brochureware” site is not vulnerable to serious reflected XSS attacks. XSS can cause a variety of problems for the end user that range in severity from an annoyance to complete account compromise. The most severe XSS attacks involve disclosure of the user’s session cookie, allowing an attacker to hijack the user’s session and take over the account. Other damaging attacks include the disclosure of end user files, installation of Trojan horse programs, redirect the user to some other page or site, or modify presentation of content. An XSS vulnerability allowing an attacker to modify a press release or news item could affect a company’s stock price or lessen consumer confidence. An XSS vulnerability on a pharmaceutical site could allow an attacker to modify dosage information resulting in an overdose. 
### Recommendation(s)
The assessment team highly recommends that any site potentially vulnerable to XSS conform to regular penetration testing.  Rigorous testing is necessary because this attack has  many variants. Sometimes, an application that properly tries to filter any malicious scripts gets confused and allows a script. Because of this we can never say that a website is fully protected. The most common recommendations are to conduct user input validation and to employ an XSS filter.    

# Finding Metadata
### Finding Development
| Author Name | Twitter Handle | Email | Created | Updated |
|:-:|:-:|:-:|:-:|:-:|
| Keelyn Roberts | @real_slacker007 |  | 05/9/2018 | 05/9/2018 |

### Finding Sources
| URL | 
|:-:|
| https://www.owasp.org/index.php/XSS_(Cross_Site_Scripting)_Prevention_Cheat_Sheet |
| https://nvd.nist.gov/download/800-53/800-53-controls.xml |
| https://www.owasp.org/index.php/Cross-site_Scripting_(XSS) |
| https://attack.mitre.org/wiki/Technique/T1203 |
| https://csrc.nist.gov/Glossary/?term=5519 |