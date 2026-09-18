```mermaid
flowchart TD

subgraph group_catalog["Catalog Core"]
    node_catalog_root["Hacking Tools Catalog<br/>[README.md]"]
end

subgraph group_recon["Discovery Assessment"]
    node_info_gathering["Information Gathering<br/>[README.md]"]
    node_vuln_analysis["Vulnerability Analysis<br/>[README.md]"]
    node_web_analysis["Web Application Analysis<br/>[README.md]"]
end

subgraph group_offense["Attack Operations"]
    node_exploitation["Exploitation Tools<br/>[README.md]"]
    node_wireless["Wireless Attacks<br/>[README.md]"]
    node_sniffing["Sniffing Spoofing<br/>[README.md]"]
    node_password_attacks["Password Attacks<br/>[README.md]"]
    node_social_engineering["Social Engineering<br/>[README.md]"]
    node_stress_testing["Stress Testing<br/>[README.md]"]
end

subgraph group_analysis["Analysis Reporting"]
    node_forensics["Forensics Tools<br/>[README.md]"]
    node_reverse_engineering["Reverse Engineering<br/>[README.md]"]
    node_reporting["Reporting Tools<br/>[README.md]"]
end

subgraph group_resources["Learning Resources"]
    node_miscellaneous["Miscellaneous Tools<br/>[README.md]"]
    node_learning_resources["Professional Resources<br/>[README.md]"]
end

node_practitioner(("Security Practitioner"))
node_nmap["Nmap"]
node_burp["Burp Suite"]
node_metasploit["Metasploit Framework"]
node_wireshark["Wireshark"]
node_ghidra["Ghidra"]
node_bugboard["BugBoard"]

node_practitioner -->|"browses"| node_catalog_root
node_catalog_root -->|"lists"| node_info_gathering
node_catalog_root -->|"lists"| node_vuln_analysis
node_catalog_root -->|"lists"| node_web_analysis
node_catalog_root -->|"lists"| node_exploitation
node_catalog_root -->|"lists"| node_wireless
node_catalog_root -->|"lists"| node_sniffing
node_catalog_root -->|"lists"| node_password_attacks
node_catalog_root -->|"lists"| node_social_engineering
node_catalog_root -->|"lists"| node_stress_testing
node_catalog_root -->|"lists"| node_forensics
node_catalog_root -->|"lists"| node_reverse_engineering
node_catalog_root -->|"lists"| node_reporting
node_catalog_root -->|"lists"| node_miscellaneous
node_catalog_root -->|"lists"| node_learning_resources
node_info_gathering -->|"features"| node_nmap
node_vuln_analysis -->|"features"| node_burp
node_vuln_analysis -->|"features"| node_nmap
node_web_analysis -->|"features"| node_burp
node_exploitation -->|"features"| node_metasploit
node_wireless -->|"features"| node_wireshark
node_sniffing -->|"features"| node_wireshark
node_reverse_engineering -->|"features"| node_ghidra
node_reporting -->|"features"| node_bugboard
node_learning_resources -.->|"supports learning"| node_practitioner

click node_catalog_root "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"
click node_info_gathering "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"
click node_vuln_analysis "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"
click node_web_analysis "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"
click node_exploitation "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"
click node_wireless "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"
click node_sniffing "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"
click node_password_attacks "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"
click node_social_engineering "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"
click node_stress_testing "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"
click node_forensics "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"
click node_reverse_engineering "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"
click node_reporting "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"
click node_miscellaneous "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"
click node_learning_resources "[https://github.com/yogsec/hacking-tools/blob/main/README.md](https://github.com/yogsec/hacking-tools/blob/main/README.md)"

classDef toneNeutral fill:#f8fafc,stroke:#334155,stroke-width:1.5px,color:#0f172a
classDef toneBlue fill:#dbeafe,stroke:#2563eb,stroke-width:1.5px,color:#172554
classDef toneAmber fill:#fef3c7,stroke:#d97706,stroke-width:1.5px,color:#78350f
classDef toneMint fill:#dcfce7,stroke:#16a34a,stroke-width:1.5px,color:#14532d
classDef toneRose fill:#ffe4e6,stroke:#e11d48,stroke-width:1.5px,color:#881337
classDef toneIndigo fill:#e0e7ff,stroke:#4f46e5,stroke-width:1.5px,color:#312e81
classDef toneTeal fill:#ccfbf1,stroke:#0f766e,stroke-width:1.5px,color:#134e4a
class node_catalog_root toneBlue
class node_info_gathering,node_vuln_analysis,node_web_analysis toneAmber
class node_exploitation,node_wireless,node_sniffing,node_password_attacks,node_social_engineering,node_stress_testing toneMint
class node_forensics,node_reverse_engineering,node_reporting toneRose
class node_miscellaneous,node_learning_resources,node_practitioner,node_nmap,node_burp,node_metasploit,node_wireshark,node_ghidra,node_bugboard toneIndigo
