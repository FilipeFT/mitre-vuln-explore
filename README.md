# MITRE vulnerabilities explorer

An effort to interface with MITRE's TAXII servers to extract information from STIX formatted vulnerabilities database

STIX is a standardized language for describing cyber threat information, including vulnerabilities, indicators of compromise (IOCs), threat actors, and more. It provides a structured and standardized way to represent, exchange, and analyze cybersecurity information. STIX uses JSON or XML as the underlying format for representing the information.

TAXII, on the other hand, is a protocol used to exchange cyber threat information between different organizations and security systems. It provides a standardized way to transport STIX content securely and efficiently. TAXII defines a set of RESTful APIs and message exchange patterns for exchanging STIX content, enabling organizations to share threat intelligence in a structured manner.

With STIX and TAXII, organizations can exchange information about vulnerabilities, threats, and other cybersecurity-related data, allowing for better collaboration and defense against cyber threats.

    a) Parsing the STIX Data:
        Obtain the STIX data from the database, which may involve accessing the database via the TAXII protocol or retrieving STIX files in JSON or XML format.
        Parse the STIX data into a suitable data structure in your programming language of choice (e.g., JSON objects, Python dictionaries, etc.). You can use libraries such as python-stix, python-stix2, or other STIX parsers based on your programming language.

    b) Extracting Technique Information:
        Identify the relevant STIX objects that represent techniques, such as Attack Patterns or TTPs (Tactics, Techniques, and Procedures).
        Extract the necessary information from these objects, such as the technique name, associated data sources, and mitigations. Pay attention to the relationships and attributes defined within the STIX objects to capture the desired information.

    c) Aggregating and Analyzing Data:
        Perform aggregations to determine the count of data sources and mitigations for each technique.
        Build data structures, such as dictionaries or maps, to store the counts of data sources and mitigations associated with each technique.
        Iterate through the parsed STIX objects and update the counts for each technique based on the data sources and mitigations associated with them.
