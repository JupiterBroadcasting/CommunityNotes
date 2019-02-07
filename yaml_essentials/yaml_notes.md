# YAML Essentials

## Introduction 

- Connect with [Ell](https://twitter.com/Ell_o_Punk) and [Elle](https://twitter.com/ellejaclyn)
  
- Free Linux Academy [community account](https://linuxacademy.com/join/community)
  - Take  [YAML Essentials](https://linuxacademy.com/devops/training/course/name/yaml-essentials) for free
  - Test your skills [**Structuring a YAML Playbook with Ansible**](https://linuxacademy.com/cp/modules/view/id/276) Free Learning Activity.
- [March Study Group](https://www.meetup.com/jupiterbroadcasting/events/258602577/)
- Vote for [April Study Group](https://tinyurl.com/aprilstudygroup) *Note: This was previously listed as voting for March study group.* 
  
### What is YAML 
 
- YAML Ain't Markup Language
  * Data serialization
  * That's really it: It's just structured data
- YAML is familiar
  * Data types you know:
    * **Lists**
        - AKA: Arrays
        - Rundown:
           * Dash-and-space
           * Can be nested
           * Cannot nest with other lists
           * Cannot be empty
           * Can contain a list of associative arrays/mappings  
           ```
            ---
            - ship: the enterprise
              crew:
                - Jean-Luc Picard
                - William Riker
                - Georgi La Forge
                
    * **Scalars**
        * Can contain strings, numbers, whitespace, Booleans
        * Convert to to string with quotes
        * 'Single quotes' are literal
        * "Double quotes" allow for escape characters (\n)
    - *Multiline Scalars:*
        * Vertical bar (|) to preserve linebreak
        * Greater than (>) to convert linebreaks to single spaces
        ```
        ---

        engineering_downtime: |
          42073.1: Navigation system upgrade
          42073.2: Holodeck maintenance

        captains_log: >
          Captain's Log, Stardate 42193.6.
          We're on a long reach toward
          the Morgana Quadrant, a section
          of the galaxy which has yet to be
          visited by a manned Federation vessel.
        ```
    * **Associative arrays**
        * AKA: 
            * Key-value pairs
            * Mappings
        * Run Down: 
            * Colon-and-a-space
            * Can be nested
            * Can contain lists
            * "Keys" cannot be duplicated*
            * Values can be empty
            ```
            ---
            
            the-enterprise:
              captain: Jean-Luc Picard
              medical:
                - Beverly Crusher
                - Katherine Pulaski

            voyager:
              captain: Katherine Janeway
              medical:
                - The Doctor
                - Kes
            ```
###  Advancing Your YAML
* Tags:
    - Allow you to expose tags to certain APIs
    - Let your apps parse your YAML the way you want
* Anchors:
    - Replicate portions of your data by assigning a reference
* Structure you know:
    * Dashes
    * Indentation (two spaces)
    * Colons
* Additional structure:
    * Signal the end of file (in one file)
    * Signal separate documents (in one file)
    ```
    ---
    crew:
      - !CAP Jean-Luc Picard
    ...
    ---
    captain: &JANE Katherine Janeway
    crew:
      - *JANE
    ---
    captain: James T. Kirk 
    ```
