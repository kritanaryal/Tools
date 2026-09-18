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

classDef toneNeutral fill:#f8fafc,stroke:#334155,stroke-width:1.5px,color:#0f1
