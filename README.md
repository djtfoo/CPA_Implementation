# CPA_Implementation
Implementation of Correlation Power Analysis (CPA) in Python to retrieve the key of an AES-128 algorithm from collected power traces, and generate plots of "correlation of all possible key bytes" and "correlation of the correct key byte vs number of traces".

## Implementation
- Written in Python 3
- Environment: Jupyter Notebook (to conveniently sectionise codes and save graph plots)

The CPA algorithm implementation codes are under the "Correlation Power Analysis (CPA)" section, "CPA Algorithm" subheader, and the plots are under the "Experimental Results Plots" section.

Various helper functions are implemented to assist in computation and accessing data from the waveform CSV. These functions are described in the report.

## How to Run
1. Ensure the following libraries are installed for the selected Python environment: pandas, numpy, tqdm, matplotlib
2. Install Jupyter Notebook
3. Open CPA_Codes.ipynb in Jupyter Notebook
4. Run through the sections of codes to open the waveform dataset, execute the definitions of helper functions, and run the algorithm

## Issues with tqdm
The tqdm library is used to print the progress bar of the codes in the CPA algorithm implementation. It might have compatibility issues with some configurations in Python and Jupyter Notebook.
If the codes fail to run, the following statements can be commented/uncommented to use a regular for loop:
- comment out the line, "from tqdm import tqdm"
- comment out the line, "for n in tqdm(range(plaintext_len), desc="Plaintext char"):"
- uncomment the line, "for n in range(plaintext_len):"
