### A Knowledge Processing Framework using Foundation Models based on RAG 
[https://arxiv.org/abs/2401.00544]

This is an example code to be included as supplementary material to the following article: 
"A Reliable Knowledge Processing Framework for Combustion Science using Foundation Models". 2024

Authors: 
    - Vansh Sharma, Venkat Raman

Affiliation: 
    - APCL Group 
    - Department of Aerospace Engineering, University of Michigan, Ann Arbor


Steps:

1. Install the packages using pip - the list is provided. It is advised to create a separate python environment for working with the code.

    Venv steps (in VS Code):
      
    a. Create environment using: Cmd + Shift + P and then Create Environment (venv)
   
    b. Activate venv using: source .venv/bin/activate
   
    c. Install packages using: pip install -r "requirements.txt"

2. Download the LLM model from link provided: https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main
      For this work you can use - llama-2-7b-chat.ggmlv3.q8_0

3. Use the correct document-data path in create_database.py file and run the code.

4. Once the database is created, update the database path in file - framework_demo.py and run the code for Q&A.

Note - the correct path to LLM model needs to be provided in framework_demo.py


Please cite this work as : 
@misc{sharma2024reliable,
      title={A Reliable Knowledge Processing Framework for Combustion Science using Foundation Models}, 
      author={Vansh Sharma and Venkat Raman},
      year={2024},
      eprint={2401.00544},
      archivePrefix={arXiv},
      primaryClass={cs.AI}
}

Additional notes on Python version and Package List
1. Code runs with Python 3.11.9 with venv
2. Omitted packages for compatibility:
    - chromaviz==0.0.4
    - gmsh==4.12.0.dev1
    - ray==2.4.0
    - urllib==31.26.16
3. Modified packages for compatibility:
    - grpcio==1.49.1 --> grpcio==1.56.0
